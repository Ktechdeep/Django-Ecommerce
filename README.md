# Django-Ecommerce

Ecommerce website built with Django 2.2.3, Python 3.7.3, and AWS/EC2

![image](https://user-images.githubusercontent.com/29988949/65267147-499fc580-dac9-11e9-90e8-eccbc93c7c3a.png)

`Product Slide`

![image](https://user-images.githubusercontent.com/29988949/65999313-ff67fe00-e451-11e9-9ed9-fc7bce704f17.png)

`Shop Page`
![image](https://user-images.githubusercontent.com/29988949/66098968-923f9000-e559-11e9-8691-cd5c2b181ca1.png)

`Product Detail Page`
![image](https://user-images.githubusercontent.com/29988949/66291084-bff84200-e895-11e9-8d53-3aa23b29dbae.png)

`Cart Page`
![image](https://user-images.githubusercontent.com/29988949/66291144-f0d87700-e895-11e9-8545-b8f93f799063.png)

`BillingAddress Page`
![image](https://user-images.githubusercontent.com/29988949/66291542-013d2180-e897-11e9-8ea9-40afcb90cee2.png)

`Stripe Payment Page`
![image](https://user-images.githubusercontent.com/29988949/66291610-29c51b80-e897-11e9-8b47-20de35d6c1d0.png)

`Order Success Page`
![image](https://user-images.githubusercontent.com/29988949/66291657-3e091880-e897-11e9-830b-6cf44e72a995.png)




# Installation

`git clone https://github.com/Ktechdeep/Django-Ecommerce.git`

`cd Django-Ecommerce`


# For Mac/ Linux/ ubuntu : Creating Environment and installing dependency

`sudo apt update`

`sudo apt install python3-venv python3-pip -y`

`python3 -m venv myenv`

`source myenv/bin/activate`

`pip install -r requirements.txt`

Install below version in terminal and 'New Version will face version conflict error'

```python

pip install Django==2.2.4
python -m pip install django-allauth==0.40.0
pip install django-crispy-forms==1.7.2
pip install django-countries==5.5
pip install stripe==2.37.1
pip install Pillow

```

`python manage.py makemigrations`

`python manage.py migrate`

`python manage.py runserver`

## (For EC2) Add New Inbound rule in security group to accept request from anywhere 
`Rule : Type: custom , PortRange : 8000 , Source : custom , 0.0.0.0`

Go to allowed host in setting.py file 
Add your EC2 instance ip in allowed host list inside setting.py file
`Allowedhost = ['YourEC2IP']`

Now open tab on anymachine:
`http://yourip:8000`

`python manage.py runserver 0.0.0.0:8000`


# For Admin Login

```python
python manage.py createsuperuser
Username : admin
Password : 12345678
```
# Demo

http://djangoecommerce.pythonanywhere.com

# HTML Template

https://colorlib.com/etc/fashe/index.html


