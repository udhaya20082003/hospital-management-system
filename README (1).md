# Hospital Management System :

This web application is designed to streamline hospital room management and prioritize patients for isolation. It serves as a centralized hub for overseeing patients and optimizing room allocation, enabling better patient care and resource management.

The platform provides nurses with real-time insights into patient details and their corresponding room assignments, ensuring efficient hospital operations.

# Prerequisites
- Node.js 6.9.1 or later - install from https://nodejs.org/

# Installing - easy :
1.	Download the repository
```
git clone https://github.com/udhaya20082003/hospital-management-system.git
```
2.	Open the Terminal (Linux & MacOS) or PowerShell (Windows) and change directory to the project folder.
3.	Type ‘npm install’ in the Terminal (PowerShell) and press Enter. All the dependencies would be installed.
4.	Go back to the Terminal (PowerShell) and be sure that you are pointing inside the project folder. To open the application, type ‘node app.js’ and press Enter.
5.	The application should be live on the local port 3000.  
6.	Type http://localhost:3000/ into a browser.
7.	To login use the username: admin  and the password: admin
8.	Now you should be inside the application
## **Features :**
1. **Patient Dashboard:**  
   - Overview of patients, their room assignments, and priority scores.  
   - Dashboard is divided into three sections:  
     - Patients with assigned rooms.  
     - Patients waiting for room allocation.  
     - Available rooms.

2. **Add New Patients:**  
   - Add a patient’s personal details and medical conditions.  
   - The system automatically calculates a priority score based on diseases.

3. **Update Patient Information:**  
   - Double-click a patient’s name on the dashboard to view their personal page.  
   - Update their diagnosis for the next 24 hours, clearing any warning flags.

4. **System Settings:**  
   - Manage hospital settings such as diseases, rooms, and user accounts.  
   - Add, delete, or update diseases and rooms.

---

## **Screenshots**
### Dashboard  
View data about patients, rooms, and their statuses:  

[corrected_hospital_management_system](https://github.com/user-attachments/assets/dd4edd03-6517-4f5c-aaac-0e7e451bfb80)

### Add Patient Page  
Add new patients and automatically calculate their scores:  

![Add Patient Page](https://github.com/user-attachments/assets/c37304c5-7b75-4208-bcb2-dcb5b458468e)

### Patient Page  
View and update a patient’s information:  

![Patient Page](https://github.com/user-attachments/assets/c0c8beee-d291-4758-a5d4-975c2da0cf5f)  

### System Settings  
Manage hospital resources, diseases, and users:  

![System Settings](https://github.com/user-attachments/assets/44202513-20b7-44a0-bb6f-5d901971e48d) 

---
 
 # App Modules and Code organisation
### Modules

Module|Core	|Patients|Diseases|Rooms 
------|-----|--------|--------|----
Functionality	|- login system | - add / delete patients | - add / delete diseases | 	- assign rooms to patients
.|- add users | - update patient's diagnosis | - assign disease to patients | - add / remove rooms
.|- view dashboard	| - view patient’s page | 
.|.| - retrieve patient's information	

### Code organisation :open_file_folder:

Folder | Content | Responsability
------|-----|--------
/public	| |	Contains the public files, such as CSS, fonts and scripts.
/routes	| |	Manage the HTTP requests. Is divided into smaller modules responsible for disjoint tasks.
.	|/app.js| 	Renders dashboard page
.	|/disease.js| 	Responsible for diseases
.	|/login.js|	Responsible for logging in
.	|/patients.js|	Responsible for patients
.	|/rooms.js|	Responsible for rooms
.	|/settings.js|	Renders settings page
.	|/users.js|	Add new users and logout
/server	| |	Defines the database and Schemas
.	|/db/mongoose.js| 	Database settings
.	|/models| 	Defines Schemas
/views		| |Render pages
.	|/layouts|	The core layout; each page is rendered inside the layout
.	|/(other files)|	Contains specific visual changes for every page

# Technologies

### Backend
Nodejs - ExpressJS

### Frontend
jQuery
### Database
MongoDB - mongoose

### Databse Schema
![Database schema](https://github.com/user-attachments/assets/912f6ff0-2c61-4627-9509-21799c8ee78b)







































