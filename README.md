# Ex04 Places Around Me
# Date:
30/09/2025
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
```
map : 

{% load static %}
<html>
    <head>
        <style>
            img{
                width:1490px;
                padding-top: 90px;
            }
            h2{
                padding-top: 60px;
            }
        </style>
    </head>
    <body bgcolor="aquamarine">
        <h2 align="center"><u>IMAGE MAP</u></h2>
        <img src="{% static 'maps1.png' %}" alt="map" usemap="#mname" >
        <map name="mname">
            <area shape="rect" coords="536,233,469,306" alt="Ractangle" href="{% url 'map1' %}">
            <area shape="rect" coords="1150,233,1220,306" alt="Ractangle" href="{% url 'map2' %}">
            <area shape="rect" coords="336,153,399,80" alt="Ractangle" href="{% url 'map3' %}">
            <area shape="rect" coords="886,633,846,586" alt="Ractangle" href="{% url 'map4' %}">
        </map>
    </body>
</html>

site1 :

{% load static %}
<html>
    <head>
        <style>
            img{
                display:block;
                margin:auto;
                width:600px;
                border:solid black 10px;
            }
            h2{
                font-family: algerian;
                font-size:40;
                width:fit-content;
                margin:auto;
            }
            p{
                width:fit-content;
                margin:auto;
                font-family: Franklin Gothic Medium;
                align:center;
                font-size: 19;
                background-color:antiquewhite;
                border-radius: 50px;
                padding:30px;
            }
        </style>
    </head>
    <body bgcolor="aquamarine">
        <h2>Sri Panjamuga Anjaneya Swami Aalayam</h2><br><br>
        <img src="{% static 'site1.avif' %}" alt="site1">
        <br><br>
        <p>Sri Panjamuga Anjaneya Swami Aalayam is a sacred Hindu temple located in Sikkarayapuram, near Mangadu in Chennai, Tamil Nadu.
            <br>This temple is renowned for its majestic 32-foot-tall statue of Lord Hanuman in his rare and<br>
             powerful five-faced (Panchamukha) form—Hanuman, Narasimha, Garuda, Varaha, and Hayagriva—each face<br>
              symbolizing divine protection, wisdom, and strength. The temple is situated at 9A, Kunrathur Road, Leelavathi Nagar, and <br>
              is approximately 3 km from the famous Mangadu Kamakshi Amman Temple
            </p>
    </body>
</html>

site2 :

{% load static %}
<html>
    <head>
        <style>
            img{
                display:block;
                margin:auto;
                width:600px;
                border:solid black 10px;
            }
            h2{
                font-family: algerian;
                font-size:40;
                width:fit-content;
                margin:auto;
            }
            p{
                width:fit-content;
                margin:auto;
                font-family: Franklin Gothic Medium;
                align:center;
                font-size: 19;
                background-color:antiquewhite;
                border-radius: 50px;
                padding:30px;
            }
        </style>
    </head>
    <body bgcolor="aquamarine">
        <h2>Sri Muthukumaran College Of Arts And Science</h2><br><br>
        <img src="{% static 'site2.avif' %}" alt="site2">
        <br><br>
        <p>Established in 2001, Sri Muthukumaran Arts and Science College (SMASC) is a private, unaided institution located in a 
            quiet, rural setting in Chikkarayapuram, Chennai.<br> Affiliated with the University of Madras, the college is part of a larger educational network run by the Sri Muthukumaran Educational Trust. <br>
            SMASC aims to offer students a supportive learning environment, helping to develop their skills and prepare them for a competitive world.
        </p>
    </body>
</html>

site3 :

{% load static %}
<html>
    <head>
        <style>
            img{
                display:block;
                margin:auto;
                width:600px;
            }
            h2{
                font-family: algerian;
                font-size:40;
                width:fit-content;
                margin:auto;
            }
            p{
                width:fit-content;
                margin:auto;
                font-family: Franklin Gothic Medium;
                align:center;
                font-size: 19;
                background-color:antiquewhite;
                border-radius: 50px;
                padding:30px;
            }
        </style>
    </head>
    <body bgcolor="aquamarine">
        <h2>Sri Sai Sarvalayam</h2><br><br>
        <img src="{% static 'site3.jpg' %}" alt="site3">
        <br><br>
        <p>Sri Sai Sarvalayam is a Hindu temple dedicated to Shirdi Sai Baba, located in the residential area of Chikkarayapuram in Chennai,<br>
            near Kovur and Mangadu. It is known for its beautiful, sparkling white marble idol of Sai Baba. <br>
            Though a more recently built temple situated in a narrow street, it is kept neat and tidy. In addition to the main deity, <br>
            the temple complex features shrines for other gods, including Ganesh, Hanuman, Nag Devtha, Sapthashringhi, Shri Triyambakeshwar, and Murugan. <br>
            It is considered a serene and peaceful place for devotees to meditate and pray to Shirdi Sai Baba.
        </p>
    </body>
</html>

site4 :

{% load static %}
<html>
    <head>
        <style>
            img{
                display:block;
                margin:auto;
                width:800px;
            }
            h2{
                font-family: algerian;
                font-size:40;
                width:fit-content;
                margin:auto;
            }
            p{
                width:fit-content;
                margin:auto;
                font-family: Franklin Gothic Medium;
                align:center;
                font-size: 19;
                background-color:antiquewhite;
                border-radius: 50px;
                padding:30px;
            }
        </style>
    </head>
    <body bgcolor="aquamarine">
        <h2>Hunters Hydraulic Scissors And Lift Manufacturers</h2><br><br>
        <img src="{% static 'site4.jpg' %}" alt="site4">
        <br><br>
        <p>Hunter Hydraulics is a Chennai-based manufacturer specializing in hydraulic material handling equipment, with its manufacturing <br>unit located in Chikkarayapuram. Operating since 2016, the company, also known as Hunter Equipments, produces a wide range <br>of goods, including various types of scissor lifts, industrial stackers, hand pallet trucks, and dock levelers. These products, which <br>include over 100 different models, are utilized across various industries, such as construction, warehousing, and <br>manufacturing, providing reliable and efficient lifting solutions. The company is recognized for its customer-centric approach and <br>commitment to producing top-quality, high-tensile strength equipment that conforms to international quality standards.
            </p>
    </body>
</html>

views.py:

from django.shortcuts import render

def fun(request):
    return render(request,"map.html")
def saitemple(request):
    return render(request,"saitemple.html")
def liftmanf(request):
    return render(request,"liftmanf.html")
def simaas(request):
    return render(request,"simaas.html")
def hanuman(request):
    return render(request,"hanumantemple.html")            

urls.py ;

from django.contrib import admin
from django.urls import path
from app import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.fun),
    path('map1/',views.saitemple,name="map1"),
    path('map2/',views.simaas,name="map2"),
    path('map3/',views.liftmanf,name="map3"),
    path('map4/',views.hanuman,name="map4"),
]

```
# OUTPUT
![alt text](<127.0.0.1_8000 - Personal - Microsoft​ Edge 30-09-2025 23_26_37.png>) 
![alt text](<127.0.0.1_8000 - Personal - Microsoft​ Edge 30-09-2025 23_26_47.png>) 
![alt text](<127.0.0.1_8000 - Personal - Microsoft​ Edge 30-09-2025 23_26_53.png>) 
![alt text](<127.0.0.1_8000 - Personal - Microsoft​ Edge 30-09-2025 23_27_05.png>) 
![alt text](<127.0.0.1_8000 - Personal - Microsoft​ Edge 30-09-2025 23_27_12.png>)


# RESULT
The program for implementing image maps using HTML is executed successfully.
