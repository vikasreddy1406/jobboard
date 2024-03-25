# JobBoard


The Job Board platform provides a way to connect job seekers with employers.
At its core, the "Job Board" project is a digital hub designed to simplify the job search process for both job seekers and companies. It provides a user-friendly interface where job seekers can explore various job opportunities and companies can effortlessly post job openings.
The project boasts a range of features, including:
●	Easy job search: Job seekers can search for jobs based on their preferences, such as industry, salary range, and location.
●	User-friendly interface: The platform offers a simple and intuitive interface for users to navigate and interact with.
●	Job posting: Companies can easily post job openings, providing detailed information about the positions available.
●	Applicant management: Employers can efficiently manage job applications received through the platform.
●	User profiles: Job seekers can create profiles to showcase their skills, experience, and qualifications.
●	Company profiles: Companies can create profiles to provide information about their organization and the positions they offer.
Overall, the "Job Board" project aims to streamline the job search and recruitment process, making it easier for job seekers to find suitable opportunities and for companies to connect with talented individuals.
 
ARCHITECTURE

The architecture of this project is broadly divided into 3 divisions:
1.	Frontend
2.	Backend
3.	Database

FRONTEND
This division contains the endpoint the user will interact with. Following is the list of pages that are present in the frontend.

1.	Home Page
2.	About Page
3.	Signup Page
4.	Login Page
5.	User Home Page
6.	User Profile Page
7.	Find Job Page
8.	Company Home Page
9.	Job Posting Page
10.	Job Info Page
11.	Applicants Page

Here is an overview of how these pages are connected.
 

Home Page
This is the home page of our website. User and Company both will start from this page. It presents a basic overview of the platform, which contains an intro, some recently posted jobs, and available tags. 
It contains Signup and Login buttons which redirect to their relevant pages, and an About button which navigates you to the About page, discussed below. It also contains a FindJob button.

About Page
This page contains information about the JobBoard platform itself,

Signup Page
This page handles signup for both the Company and the User. Most of the information like email, password, resume, location, and description is asked at this point.
 
For the description field, we provide both the User and Company with options to format their description to help them stand out in the competition.

Login Page
This page handles login for both the Company and the User. Both the Company and the User provide their email and password. Relevant notifications are shown in case of incorrect or empty information to improve user experience.
 

User Home Page
The User Home Page is similar to the Home Page except it's slightly modified for the user. This is done to avoid many transitions and make it easy for the User to use the platform.
User Profile Page
This page contains information about the user, like the user's image, email, contact info, description, and resume. It also presents the user with a button to download the resume in `pdf` format.
 

Find Job Page
This page allows users to search through jobs according to their needs. To achieve this there are various filter options available like industry, salary range, location, and skills required.
The job cards contain a button to navigate to the Job Info page which provides more information and functionalities described below.

Company Home Page
Contains details about the company like, email, contact email, recently posted jobs, location, owner.
This page also acts as Company Profile Page when user wants to see the details of the company.
 
 

Job Posting Page
This page is only available to companies and not to users. Companies can enter the job details in the relevant fields, and if the company needs to provide job details for which no relevant field exists, that information can be entered into the description box. The description box provides various formatting tools to handle large information with good formatting.
 

Job Info Page
This page contains detailed information about the job. Both user and company can see this page to get detailed information about the job.
When the company who posted this job is viewing this page. It will be provided with an option to see the applicants, and if the user is viewing the job, then an apply button will be presented to the user.
 

Applicants Page
This page lists all applicants who applied for the job. This page is accessible only to companies through the job info page. The user name acts as link, which redirects the company to the User Profile page where the company can see more about its detail and can download the resume. A download resume button is also provided in the applicants page itself for easy downloading of the resume.
  

 
BACKEND
The API is designed according to the REST API and follows the best practices and guide
The server is stateless and the api is divided by the resources as specified by the REST API conventions. For example, this will create a user with the specified details.
 
For instance, following is the list of APIs available for the user resource.  


DATABASE
For the database we have used Postgres as it is an open source and cross-platform package which offers the most features and control than its competitors.
Database is implemented using the following schema. The users_jobs table is used to maintain many-to-many relationship between users and jobs without causing redundancy.
 
To connect backend with the database, we used sequelize. Sequelize is javascript package which hides the physical database under an ORM layer and provides object oriented approach to access the database. This also allows to change the database without changing the source code. 
COLLABORATION

Collaboration was a big challenge, considering the diversity in region and timing. To resolve these we used various tools to help track and contribute to the project.
For source code collboration, we used to git and github, a well renowned combination in the software development field. For task management we used the trello board, and for visual representation of the components and structure of the project and the inter connection between them, use used miro, which is a very easy to use diagram tool.

 
TECHNOLOGY STACK

FRONTEND
-	HTML
-	CSS
-	JavaScript
-	ReactJs

BACKEND
-	NodeJs
-	ExpressJs
-	Sequelize

DATABASE
-	Postgres

MANAGEMENT & COLLOBORATION
-	Git and GitHub
-	Trello
-	Miro
 
FUTURE WORK

While the "Job Board" project has made significant strides in revolutionizing the job search and recruitment process, there are several areas identified for further enhancement and improvement. Below are some key ideas for future work:
●	Simplified Signup UI:
Revamp signup interface for smoother registration, reducing mandatory fields and providing clearer instructions.
●	GitHub Actions Integration:
Automate testing and deployment using GitHub Actions to improve development workflow efficiency and code reliability.
●	Job Deletion Feature:
Enable companies to delete outdated job postings, ensuring job listings remain up-to-date for users.
●	Enhanced Loading UI:
Implement loading indicators like spinners or progress bars to keep users informed during data loading processes.
●	Reduced Signup Requirements:
Minimize mandatory fields in signup forms to simplify the signup process for all users.
●	Session Management:
Enhance security and user experience with robust session management functionalities.
 
TEAM MEMBERS

-	Chetan Singh Sajwan
	Backend, Database
-	Shivkesh Pandey
Frontend, Databse
-	Lovish Malhotra
Frontend, Backend
-	Sai Vikas Reddy
Frontend
-	Suresh Kumar
Frontend
-	Hari Raj
Frontend
-	Santosh S
Frontend
 
CONCLUSION

The "Job Board" project is all about making it easier for people to find jobs and for companies to find the right employees. We've built a place where job seekers and employers can meet up, making the whole process of getting a job or hiring someone a lot simpler.
We're proud of what we've achieved, but we know there's always room to do even better. We plan to keep improving, adding new features, and listening to what our users need.
In short, our project uses tech to solve real-world job search problems, making the process smoother for everyone involved. We're excited to keep growing and helping more people find their perfect job match.

