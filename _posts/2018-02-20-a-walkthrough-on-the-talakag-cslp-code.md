---
layout: post
title: "A Walkthrough on the Talakag CSLP Code"
categories:
  - Projects
  - Web-Development
description: 
image: /assets/images/posts/talakag-db-code.jpg
---

> The move towards a unified agricultural market helps farmers get correct remuneration for their produce &mdash; Arundhati Bhattacharya

It is our concern to help our farmers in their produce by helping the farmers near our locality to create a new tool for faster insurance registration. Good thing that Xavier University has conducted the Collaborative Service Learning Program or CSLP, we will then be able to reach out to our farmers who are in dire need of a fast insurance application system.

The Registry System for Basic Sectors in Agriculture – Philippine Crop Insurance Corporation (RSBSA-PCIC) Database and Bulk SMS for Talakag Farmers is a collection of database of the farmers who have opted to apply for an application for insurance. The project is hoped as an automated web application to accomplish the task of registration, assessment of application documents, and application renewal. The insurance is to be renewed every after crops or livestock are planted and should be made available on the present year that the application was provided. 

> The registry system collects the personal information of the applicant together with the other pertinent information deemed to be important for the processing of their application. 

The project at first was to develop a database of the collection of farmers all around the Municipality of Talakag, however, the project was already accomplished, and thus, need to work on an another project which is the RSBSA-PCIC Database. Together with the database, we are to create an automated Bulk SMS System for Talakag farmers in hopes to address the difficulty of transporting and sending information of farmers across Talakag. It should message in bulk based in the categories selected by the user which is the Talakag MAO.

In the project, we have two types of application forms to be made into a web application, namely the Application Form for Livestock Mortality Insurance (PPP) and the Application Form for Crop Insurance (Group Application). 

![PCIC Application Forms](/assets/images/posts/body/talakag_app.jpg "PCIC Application Forms")

Below shows the code of the variable declarations for **Application Form for Livestock Mortality Insurance (PPP)**
<details style="margin-bottom: 30px;">
	<summary style="background: #9f8f68; color: #fff; padding: 1em; cursor: pointer; border-radius: 0.3rem; font-weight: bold; box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);">Click to show code</summary>
	<script src="https://gist.github.com/marcreyesph/f6b83af5857fea96d4bc0b793e3d11bb.js"></script>
</details>

On the other hand, the code below shows the Application Form for **Crop Insurance (Group Application)**
<details style="margin-bottom: 30px;">
	<summary style="background: #9f8f68; color: #fff; padding: 1em; cursor: pointer; border-radius: 0.3rem; font-weight: bold; box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);">Click to show code</summary>
	<script src="https://gist.github.com/marcreyesph/d5c50a7c6051d7547dfacb7435ab5108.js"></script>
</details>

The application forms are being saved and shown with the recent application dashboard, as a result of the application form code that is shown on the preceding section. 
![PCIC Application Dashboard](/assets/images/posts/body/talakag_dash1.jpg "PCIC Application Dashboard")

![PCIC Application Dashboard](/assets/images/posts/body/talakag_dash2.jpg "PCIC Application Dashboard")

I must say that the experience that we have had with our clients is worthwhile, memorable, and life-changing. Not only does it teach developers like me who are starting to develop applications but also to be a catalyst of the change that everyone is looking forward to. Helping our farmers would mean that we have contributed a lot to the societal progress as our farmers are the main food provider of us Filipinos. This project should encourage the youth to participate in nation bulding and helping out farmers to increase farmer production by providing a system that will help them be insured right away without having to woory about delayed or misplaced files.

![Talakag CSLP Developers](/assets/images/posts/body/talakag_all_devs.jpg "Talakag CSLP Developers")

---

The project is currently on its beta release and we would want to listen on what you think about our project. Feel free to e-mail me at **[hello@marcreyes.ph](mailto:hello@marcreyes.ph)** to inquire more about this project and to also help our farmers more. 


