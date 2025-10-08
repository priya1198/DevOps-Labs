The goal of this project is to set up a Java build environment using Maven and deploy the resulting .war file to a Tomcat server running on another EC2 instance.

1. Created Two AWS EC2 Instances

> One instance for build

> One instance for deployment

Screenshot: 

<img width="1069" height="279" alt="Image" src="https://github.com/user-attachments/assets/98263f35-cbdc-455d-8104-6059bf04b70d" />


2. Connected to Instances Using SSH

Connected both EC2 instances from a terminal using SSH (each in a separate tab).

Screenshot: 

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/23abda54-8d9a-499a-aa1f-c06171b588da" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/5d69b617-2e6f-4e89-b427-130ec0bed571" />

<img width="1059" height="277" alt="Image" src="https://github.com/user-attachments/assets/adca5c67-0125-4a96-935b-e869e5b1860e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9efb1704-a58a-4a60-8e67-b4345923515d" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/5eb29cdd-683b-4b63-b892-7d37d658b740" />



3. Updated the System

>  to make sure all packages are up to date.
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/64d9c3cc-67d4-4ad8-9a60-814166bbc2e0" />

4.Build Server Configuration

>  Installed Java 17

Downloaded and installed Java 17 to support Java-based projects.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/8e41775b-b696-4f7e-b840-37fed3ccb883" />



5. Installed Maven

> Set up Maven to manage and build the Java project.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f8860a7d-ef6c-476e-909a-bcd632d7d2af" />



6. Cloned Java Code from GitHub

> Pulled the Java source code from a remote Git repository into the build server.

<img width="766" height="288" alt="Image" src="https://github.com/user-attachments/assets/03ee0645-bd5d-43e9-8c96-4116307a86de" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ec743507-0f6e-49d8-88fe-a69718e6beb2" />



7.Validated Maven Project

> Ran Maven validation to ensure the project setup is correct.



8. Build Failure Encountered

> Initial build failed due to configuration issues in the pom.xml file.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4587ea22-2c75-4ff1-b150-b3051c76b286" />



9. Fixed the pom.xml File

> Manually edited the pom.xml to fix dependency or plugin issues.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ec85ea77-679a-43de-80b0-b90077c625fa" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e9a79060-6d73-4c18-8502-12f4b33ef325" />



10. Built the Project

> Re-ran the Maven build and successfully generated the .war file.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9e25abc5-997f-4545-99e2-e695da7bf53c" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/647662fb-ccbc-4924-afb1-2a4b5d019640" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/6d235359-9448-4d81-a07f-ce618e5b030c" />



12. Updated the Deployment Server

> Updated all system packages on the deploy server.
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/3a3d62a2-7e44-42fa-8cf7-f28d7f56ca89" />



13. Installed Java

> Installed Java to run Tomcat and Java applications.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2cf911df-3d9c-4696-8c1c-71f158185c7f" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c9331d43-6e11-4090-a100-6ccf3aaa61da" />



14. Downloaded Tomcat

> Manually downloaded Apache Tomcat from the browser.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/3b9a2bdc-95d0-4ad3-8140-6b01cacdd47e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/6f2499ef-820f-44f9-a8c7-047d48a5fa3e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a853eb6f-8bac-4a3b-89cf-31ce73fbc57a" />



15. Extracted Tomcat Files

> Unzipped the downloaded Tomcat tar/zip file.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0c1d5c0a-e0ba-4926-b9a7-f940ee413481" />



16. Started Apache Tomcat

> Navigated to the bin folder and started the Tomcat server.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/3f2de733-5972-4396-8439-4a6f685b8c39" />



17. Configured AWS Security Group (Port 8080)

> Added an inbound rule for port 8080 in the AWS EC2 security group.

<img width="1074" height="367" alt="Image" src="https://github.com/user-attachments/assets/b51aa727-c1e6-4adf-8fe2-ce7fbb8e22f6" />

<img width="1057" height="322" alt="Image" src="https://github.com/user-attachments/assets/2cc737a1-cbb9-4d0c-9ff0-c622f4f14750" />

<img width="1058" height="417" alt="Image" src="https://github.com/user-attachments/assets/b0db8c9c-dd82-45ed-b6e1-b645e8ba0437" />

<img width="1029" height="262" alt="Image" src="https://github.com/user-attachments/assets/0ff7fdc2-015f-4557-b650-26d7d437e172" />

<img width="766" height="288" alt="Image" src="https://github.com/user-attachments/assets/da402e31-874a-4409-9901-6084cf1d55b1" />



18. Accessed Tomcat Webpage in Browser

> Opened the deploy server's public IP in the browser with port 8080.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7e3e8b5b-3786-461f-bdd6-02c01a78f84e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fb15da61-f218-49df-96ea-3f8ccb230bb4" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fb2cf7e8-c094-4ae8-b51d-1a85576737e9" />



19. Edited Tomcat Context File

> Modified the context.xml to allow access to the manager app.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0652832c-6d77-42dc-9331-97a017796b31" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/070fa964-2db7-4565-8967-539a35129a46" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f4f123ee-00ab-42dd-8b8f-82bf8ab16406" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0228aac2-b932-4d64-a55b-4f7f5924daf8" />



20. Edited Tomcat Users File

> Navigated to the conf directory and opened tomcat-users.xml.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4f035b0d-06dc-4960-807d-477707110a1d" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1a991285-bf27-4f9d-8765-7440e4a821a2" />



21. Added Roles and Credentials

> Added a new role and user credentials to allow login to the manager UI.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/aa681a73-aa3d-4bca-85fa-20ee1beb0eda" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/914c89ea-acc9-4cf1-a473-5d3c47854703" />



22. Accessed Tomcat Manager UI

> Refreshed the browser and successfully accessed the Tomcat Manager Web UI.

 Screenshot: Tomcat Manager login page
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e1713c4f-07fe-4595-9a7c-aef4af4f43ba" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a06222e6-7607-4a7b-9909-2281f3ae0027" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7294a838-d1ee-4d6d-8a37-0f94d417e2a8" />

### Application Deployment



23. Copied .pem File to Build Server

> Transferred the PEM key file from the local system to the build server.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/30012760-7c53-4e9f-b393-737a3ae38194" />



24. Verified .pem File on Build Server

> Confirmed the file exists and is ready to be used for connecting to the deploy server.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/41c3e8fb-0860-4075-9426-8a8e06068740" />



25. Verified .war File is Ready

> Confirmed the .war file is available in the target/ folder.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/3c7fe9df-51a2-4e5c-99ba-895071763b72" />



26. Copied .war File to Deploy Server

> Transferred the built .war file from the build server to the webapps directory of the deploy server.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c0eb01f4-d6e7-4b9a-80ad-16640aff26ee" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/47c4232a-79f4-4366-ba1f-008c05e9153c" />



27. Deployed Web Application

> Refreshed the Tomcat webapps section in the browser and verified the deployed application.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4dcb0af4-9753-45cc-a847-ce75a3ca688a" />



28. Verified Calculator Page

> Opened the deployed application in the browser and reached the Calculator web page.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f9459c40-5d8e-47fe-8398-b671edd5dd06" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/cd0d60b9-830d-47ef-b5a2-85bf175e95ce" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/dbd640ac-46f4-4c62-989d-08573f64241e" />

### Final Outcome

> Successfully deployed the Java web application to Tomcat running on an AWS EC2 instance.



