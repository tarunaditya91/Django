# Django

# Project Overview

draw your project in a pice of paper and list out all the features on that for your idea

![img1-web](https://github.com/tarunaditya91/Django/assets/113850656/bff01b54-73cb-4690-bf4a-257196592af1)

![img2-web](https://github.com/tarunaditya91/Django/assets/113850656/8260ba94-f52d-4baa-8153-97376f26e291)

![img3_web](https://github.com/tarunaditya91/Django/assets/113850656/ffa3cb34-56b9-4d3b-8a75-27a02ceb62ac)


# Desiging in figma 

![image](https://github.com/tarunaditya91/Django/assets/113850656/7ea6c89e-9239-4c97-b9a8-9161af63db3f)

# code

after desiging the project in figma go to vs code and code the template  code the temlate useing html and css for making it responsive use @media(){} 

create venv for django and install all the pakages in it and in django app add the static and template folder int static add images and style in templatess add html files also link the css file to html  in django methid as {% static 'style/main.css' %} 



now add the path and views.py  to that page 
aftr that create three moodel Skill,Project,Tag  you will see that i have imported uuid it will provide a 16 digit number which can not be duplicated so we use this for id

class Project(models.Model):
    title=models.CharField(max_length=200)
    thubnail=models.ImageField(null=True)
    body=models.TextField()
    slug=models.SlugField(null=True,blank=True)
    created=models.DateTimeField(auto_now_add=True)
    id=models.UUIDField(default=uuid.uuid4,unique=True,primary_key=True,editable=False)


    def __str__(self):
        return self.title



  after running the cmd commands add it to the frontend to over html page





