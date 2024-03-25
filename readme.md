# JobBoard

## INTRODUCTION

The Job Board platform provides a way to connect job seekers with employers. At its core, the "Job Board" project is a digital hub designed to simplify the job search process for both job seekers and companies. It provides a user-friendly interface where job seekers can explore various job opportunities and companies can effortlessly post job openings.

The project boasts a range of features, including:

- **Easy job search:** Job seekers can search for jobs based on their preferences, such as industry, salary range, and location.
- **User-friendly interface:** The platform offers a simple and intuitive interface for users to navigate and interact with.
- **Job posting:** Companies can easily post job openings, providing detailed information about the positions available.
- **Applicant management:** Employers can efficiently manage job applications received through the platform.
- **User profiles:** Job seekers can create profiles to showcase their skills, experience, and qualifications.
- **Company profiles:** Companies can create profiles to provide information about their organization and the positions they offer.

Overall, the "Job Board" project aims to streamline the job search and recruitment process, making it easier for job seekers to find suitable opportunities and for companies to connect with talented individuals.

## Architecture

The architecture of this project is broadly divided into 3 divisions:

1. Frontend
2. Backend
3. Database

### Frontend

This division contains the endpoint the user will interact with. Following is the list of pages that are present in the frontend:

1. Home Page
2. About Page
3. Signup Page
4. Login Page
5. User Home Page
6. User Profile Page
7. Find Job Page
8. Company Home Page
9. Job Posting Page
10. Job Info Page
11. Applicants Page

Here is an overview of how these pages are connected.
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/e0f36247-757d-4b79-9f10-67c809ed5b24)

#### Home Page
This is the home page of our website. User and Company both will start from this page. It presents a basic overview of the platform, which contains an intro, some recently posted jobs, and available tags. 
It contains Signup and Login buttons which redirect to their relevant pages, and an About button which navigates you to the About page, discussed below. It also contains a FindJob button.

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/690e61e1-23d8-491c-8d71-74232aa4f739)


#### About Page
This page contains information about the JobBoard platform itself


#### Signup Page
This page handles signup for both the Company and the User. Most of the information like email, password, resume, location, and description is asked at this point.
 
For the description field, we provide both the User and Company with options to format their description to help them stand out in the competition.

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/04803b37-7a5a-4b67-901b-fb47647d7c6d)


#### Login Page
This page handles login for both the Company and the User. Both the Company and the User provide their email and password. Relevant notifications are shown in case of incorrect or empty information to improve user experience.
 
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/7d52c098-76a3-44ef-a9e2-5577328311f6)

#### User Home Page
The User Home Page is similar to the Home Page except it's slightly modified for the user. This is done to avoid many transitions and make it easy for the User to use the platform.

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/d877b5b2-d1bc-4cd8-ae96-28694cfbc289)

#### User Profile Page
This page contains information about the user, like the user's image, email, contact info, description, and resume. It also presents the user with a button to download the resume in `pdf` format.
 
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/9b33bd59-eaa7-4e3c-b7e4-249669afe2fc)

#### Find Job Page
This page allows users to search through jobs according to their needs. To achieve this there are various filter options available like industry, salary range, location, and skills required.
The job cards contain a button to navigate to the Job Info page which provides more information and functionalities described below.

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/dcd8b0b8-8bc0-4b5d-94ea-b2f3bf38240f)
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/d428abc5-aa6c-4106-a4c7-74e706a32367)


#### Company Home Page
Contains details about the company like, email, contact email, recently posted jobs, location, owner.
This page also acts as Company Profile Page when user wants to see the details of the company.
 
 ![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/f143ddf2-a4fe-499d-89d3-af91f3e12b0d)

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/9473b3fa-4308-45ef-bb9e-804710bdf47e)


#### Job Posting Page
This page is only available to companies and not to users. Companies can enter the job details in the relevant fields, and if the company needs to provide job details for which no relevant field exists, that information can be entered into the description box. The description box provides various formatting tools to handle large information with good formatting.
 
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/40400a24-0e30-4356-91ae-6ef95fe198f5)


#### Job Info Page
This page contains detailed information about the job. Both user and company can see this page to get detailed information about the job.
When the company who posted this job is viewing this page. It will be provided with an option to see the applicants, and if the user is viewing the job, then an apply button will be presented to the user.
 
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/dbd06abe-5bed-4261-85e6-a04dc55078f5)


#### Applicants Page
This page lists all applicants who applied for the job. This page is accessible only to companies through the job info page. The user name acts as link, which redirects the company to the User Profile page where the company can see more about its detail and can download the resume. A download resume button is also provided in the applicants page itself for easy downloading of the resume.
  
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/6540019a-8797-42a4-891b-84ebe5abcb2f)
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/f8ae5156-8a93-430d-b2b3-a6690845b4eb)




### Backend

The API is designed according to the REST API and follows the best practices and guides. The server is stateless and the API is divided by the resources as specified by the REST API conventions.
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/cb6ae429-dd9b-403a-a396-42a26aee4726)

For instance, following is the list of APIs available for the user resource. 
![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/2be073e3-b38b-4162-935f-e658aff187a8)

### Database

For the database, we have used Postgres. Database is implemented using the following schema. To connect backend with the database, we used Sequelize.

![image](https://github.com/vikasreddy1406/jobboard/assets/96761217/8c3125c5-1c77-4a51-9e0f-e0bd2315056d)

## Collaboration

Collaboration was a big challenge, considering the diversity in region and timing. To resolve these we used various tools to help track and contribute to the project. For source code collaboration, we used Git and GitHub. For task management, we used Trello. For visual representation of the components and structure of the project and the interconnection between them, we used Miro.

## Technology Stack

### Frontend

- HTML
- CSS
- JavaScript
- ReactJs

### Backend

- NodeJs
- ExpressJs
- Sequelize

### Database

- Postgres

### Management & Collaboration

- Git and GitHub
- Trello
- Miro

## Future Work

While the "Job Board" project has made significant strides in revolutionizing the job search and recruitment process, there are several areas identified for further enhancement and improvement. Below are some key ideas for future work:

- **Simplified Signup UI:** Revamp signup interface for smoother registration, reducing mandatory fields and providing clearer instructions.
- **GitHub Actions Integration:** Automate testing and deployment using GitHub Actions to improve development workflow efficiency and code reliability.
- **Job Deletion Feature:** Enable companies to delete outdated job postings, ensuring job listings remain up-to-date for users.
- **Enhanced Loading UI:** Implement loading indicators like spinners or progress bars to keep users informed during data loading processes.
- **Reduced Signup Requirements:** Minimize mandatory fields in signup forms to simplify the signup process for all users.
- **Session Management:** Enhance security and user experience with robust session management functionalities.

## Team Members

- Chetan Singh Sajwan (Backend, Database)
- Sai Vikas Reddy (Frontend, Backend)
- Shivkesh Pandey (Frontend, Database)
- Lovish Malhotra (Frontend, Backend)
- Suresh Kumar (Frontend)
- Hari Raj (Frontend)
- Santosh S (Frontend)

## Conclusion

The "Job Board" project is all about making it easier for people to find jobs and for companies to find the right employees. We've built a place where job seekers and employers can meet up, making the whole process of getting a job or hiring someone a lot simpler.

We're proud of what we've achieved, but we know there's always room to do even better. We plan to keep improving, adding new features, and listening to what our users need.

In short, our project uses tech to solve real-world job search problems, making the process smoother for everyone involved. We're excited to keep growing and helping more people find their perfect job match.
