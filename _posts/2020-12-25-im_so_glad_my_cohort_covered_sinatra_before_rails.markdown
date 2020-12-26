---
layout: post
title:      "I'm so glad my cohort covered Sinatra before Rails..."
date:       2020-12-26 04:20:56 +0000
permalink:  im_so_glad_my_cohort_covered_sinatra_before_rails
---


Let's just say, Rails is Sinatra on steroids!! Completing this Rails project further solidified what I learned in Sinatra including: SQL, MVC, CRUD, Restful Routing just to name a few! So, about my Rails Application...here's the story...

The receptionist for InstaStyle Medspa walked out and now the stylists have to take turns being the receptionist! Not only do they schedule their own appointments, but they also have to schedule appointments for their fellow stylists. They have asked me (their software developer) to create a web app where they can sign up/log in and create, retrieve, update, and delete appointments for their clients. Not only will this web application have CRUD capabilities for the appointments model but the stylist (user) can also make appointments for existing clients in the database or create new ones. The same is true for the service.

Now that you have run down, you see how connected this app is. The database, the models, the controllers, the views all have their part to play and I did face a few challenges. Through these challenges, I did learn a lot! One of the main things that I gained clarity on was custom setter methods for nested attributes. When using a custom method versus the macro "accepts_nested_attributes_for" you can ensure that your nested forms will process the data entered by the user correctly and that it will be rendered to the views correctly. For example, my setter method for service attributes in my Appointment Model (belong_to :service), will allow the user to enter a new service or even enter a service that belongs in the database and the method will look to see if the service name exists. If it does it will find that service name and set the value to that service name, otherwise it will create a new one.


```
 def service_attributes=(attr)
        if !attr[:name].blank?
            self.service= Service.find_or_create_by(name: attr[:name].titleize)
        end
    end
    
```


I felt really connected with my classmates during Mod 3. I think I am finally coming out of my shell and feeling more comfortable to ask questions or for help when I need it. I also felt comfortable to share my own discoveries with fellow classmates. What a wonderful time to feel connected. Thank you for visiting. Happy Holidays! 

https://github.com/Kiki1022/kshah_rails.git

