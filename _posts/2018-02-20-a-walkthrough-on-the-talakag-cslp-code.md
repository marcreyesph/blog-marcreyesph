---
layout: post
title: "A Walkthrough on the Talakag CSLP Code"
categories:
  - Projects
  - Web-Development
description: The Registry System for Basic Sectors in Agriculture – Philippine Crop Insurance Corporation (RSBSA-PCIC) Database and Bulk SMS for Talakag Farmers is a collection of database of the farmers who have opted to apply for an application for insurance. Learn more about this project by reading my blog.
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


In the other hand we have another project named FarmSend, FarmSend is a mobile application which can be installed in Android phones. This application can be used for sending messages to the farmers to inform them such as meetings, seminars and other agricultural rks related topics. It needs cellular networks like Globe/TM, Smart/TnT, and Sun. This application includes six categories; Barangay. Crops, Livestocks, Civil Status, Gender and Types of Insurance.
![FarmSend User Interface](/assets/images/posts/body/farm-send-ui.jpg "FarmSend User Interface")

To be able to start using the application, you must allow FarmSend to allow sending permissions so that it can access the messaging system. This will let FarmSend to be able to access start sending messages in bulk.
![FarmSend Allowing Permissions](/assets/images/posts/body/farm-send-perm.jpg "FarmSend Allowing Permissions")

The application below shows the selection of categories based on the user input the web application. Only in the web application in the webiste that a administrator can add a new contact and have it added onto the FarmSend database. It show the categories in Barangay. Crops, Livestocks, Civil Status, Gender and Types of Insurance.
![FarmSend Sending Categories](/assets/images/posts/body/farm-send-categories.jpg "FarmSend Sending Categories")

Prior to sending the bulk messages as it is being connected onto the same IP address as the web server, you will be able to see the confirmation as to what the recipient names are and also the included message in the said bulk message. After clicking yes, the mobile application will attempt to send the message three times if its fails the first or second attempts. The mobile application will notify if all the messages have already been sent.
![FarmSend Sending Confirmation](/assets/images/posts/body/farm-send-conf.jpg "FarmSend Sending Confirmation")

To create the mobile application, we have used Android Studio which is the recommended IDE for developing Android applications. The code snippet below shows tha MainActivity view which is the user interface that the Android application will load on application boot time. 
<details style="margin-bottom: 30px;">
	<summary style="background: #9f8f68; color: #fff; padding: 1em; cursor: pointer; border-radius: 0.3rem; font-weight: bold; box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);">Click to show code</summary>
	<script src="https://gist.github.com/marcreyesph/3de4d237a0c60cb9d09fed44cecf641a.js"></script>
</details>

On the other hand, the code below shows the BackgroundTasks which is assigned in the back-end functionalities of the application while showing the MainActivity that is being loaded on application boot time.
<details style="margin-bottom: 30px;">
	<summary style="background: #9f8f68; color: #fff; padding: 1em; cursor: pointer; border-radius: 0.3rem; font-weight: bold; box-shadow: 0 2px 5px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12);">Click to show code</summary>
	<script src="https://gist.github.com/marcreyesph/3909409e8d87830bcd86c726484897fe.js"></script>
</details>

> "Being able to reach out to farmers with our specialties while also learning process is an enjoyable thing to have." &mdash; Marc Anthony Reyes

> "We not only did this for the accomplishment of a high grade but to also help the community we have served." &mdash; Ricky Bantonare

> "We can learn new things outside the box." &mdash; Julius Urot

> "Working alone is stupid." &mdash; Romel Niño Paano

> "While doing the project, I forgot that I'm working for a school project. It just feels that I'm working for a cause, a rippling change." &mdash; Marvin Kao

> "Very honored to have helped our farmers in Talakag, Bukidnon&mdash;a thing that I will never forget." &mdash; Kathrina Ira Mitchell

I must say that the experience that we have had with our clients is worthwhile, memorable, and life-changing. Not only does it teach developers like me who are starting to develop applications but also to be a catalyst of the change that everyone is looking forward to. Helping our farmers would mean that we have contributed a lot to the societal progress as our farmers are the main food provider of us Filipinos. This project should encourage the youth to participate in nation bulding and helping out farmers to increase farmer production by providing a system that will help them be insured right away without having to woory about delayed or misplaced files.

![Talakag CSLP Developers](/assets/images/posts/body/talakag_all_devs.jpg "Talakag CSLP Developers")

---

**Project Developers**: Ricky Bantonare Marvin Kao, Kathrina Ira Mitchell, Romel Niño Paano, Marc Anthony Reyes, Julius Urot

**Open Source Integrations:** Xportability/css-to-pdf ([https://github.com/Xportability/css-to-pdf](https://github.com/Xportability/css-to-pdf)), Dogfalo/materialize ([https://github.com/Dogfalo/materialize](https://github.com/Dogfalo/materialize)), DataTables ([https://datatables.net/license/mit](https://datatables.net/license/mit)).

The developers would like to acknowledge the following for making this project possible: God, for giving us the skills and resources to begin this project, our families who are of continued support for us to be able to comply with this requirement, Talakag Registry System for Basic Sectors in Agriculture - Philippine Crop Insurance Corporation (RSBSA-PCIC) MAO, Municipality of Talakag, Ms. Amor Cajilla of CS 33.1 Software Engineering AY 2017-2018, Mr. Jessie Christopher Lagrosas of CS 32.1 Web Programming AY 2017-2018, Engr., Maria Ramila Jimenez, MIT of CS 27 Network Principles AY 2017-2018.

This project is made in fulfillment of the final requirements in CS 33.1 Software Engineering, CS 32.1 Web Programming, and CS 27 Network Principles AY 2017-2018 of Xavier University Collaborative Service Learning Program (XU-CSLP).

The project is currently on its beta release and we would want to listen on what you think about our project. Give it a try by visiting **[http://cslp.xu.edu.ph/talakag_pcic](http://cslp.xu.edu.ph/talakag_pcic)**. Feel free to e-mail me at **[hello@marcreyes.ph](mailto:hello@marcreyes.ph)** for the test log in details and to also inquire more about this project to help our farmers more. 


