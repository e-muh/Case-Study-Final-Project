# Case-Study-Final-Project

# Project name

ESAYLEARN - The Student Best Companion.

# Description

This is a mini Learning Management System (LMS) software that can be adopted by a college department to manage
the flow of her activities. It is a Spring MVC project. It targets three principal users: enrolled/unenrolled students, teachers/lecturers, 
and the system administrators responsible for coordinating the overall activities. Each user has been deligated 
specific set of actions they can perform within the system:

Students are able to login using their registration ID, password and select userType "student" and be able to:
register for courses, list all open courses for enrolment, check their registered courses. When fully completed additional functionalities such
as checking grades, download of course materials, submission of assignments, check all courses registered and completed,
send complaints on events of wrong/omitted grades, name spelling, etc. will be added.


Admins will be able to login in with their employment ID, password and select userType "admin" and be able to:
check students enrolments, create, read, update and delete users, students courses, check courses an individual student has registerd,
and additional (when project fully completed) will compile individual students report, disable student record in case
of dismissal, and many other administrative transactions

Teachers. At this stage teachers as users has not been implemented. When implemented, teachers will be able to login in with their employment ID,
 password and select userType "admin" and be able to: check courses assigned to them (approve or declined), check the course enrolment, set students grades, etc.

This project is design and implemented with a custom security freature. All users must have an account with thier user name, user password and user type stored
in the users table of the project MySQL databale. Wen a user enters his/her login credentials, the system pulls the record partaining to that credential from 
the database. If the user name, user password and user type matches with the record from the database, and based on the user type, the user will be redirected
to the student dashboard, admin dashboard, or teacher dashboard for student, admin, and teacher users respectively. If the record does not match, the user will
be redirected to the login form where the user can either: enter the correct credentials, change their password if forgotten, or create an account if they do not
do not have one. With is custom security verification and user authorization, spring security is not envisage for this project.

Currently, this project has not been fully implemented, only students and admims users has been implemented to above 80%. The requirements keep increasing
as development proceeds. As such, this project follows the Agile development model, with iterational development and delivery. The next version of this project
will have much more additional functionalites included. Stay tune.....

Also, we have a link on the hompage for the RESTful implementation of this project. Here, only the CRUD for the course POJO is implemented.


# Built With
This project is built with the following tools:

	
	Eclipse JEE
	Maven
	Apache Tomcat (Server)
	Spring MVC
	JPA/Hibernate/ORM
	MySQL Database
	JUnit 4
	JSP/JSTL (views)
	HTML4/CSS3/JavaScript
	Hibernate Validator
	PostMan (RESTful implementation)
	XML configuration(spring mvc)
	Java Configuration (REST)


# Installation

This project is deveoped on a window computer. You will need the tools above installed on your pc before you can run the project.
Additional its includes hibernate/orm and the entities are mapped as follows:

User : not mapped to any other entity. isolated.
Student : @OneToMany mapped to the course entity
Course : mapping not specified.

Apart from these, no other specific installation requirement is needed as of now. However, ensure your database name is "easylearn". 
Any other custom name for the database will require the database name to be changed on all configuration settings for the project.


# Roadmap
This is just the first version of this project, the project will be updated continuously over time. Several versions is expected in the future.


#Usage
This project is intended for academic purposes only. However, it can be upgraded into a resource management tool for vibrant businesses.


# License
This is intended to be an open source project, except otherwise decided to be licensed upon completion.


# Project stutus

This project is still in progress.


# Acknowledgement

This project is completed thanks to the generous training support of PerScholas in collaboration with TEKsystems.
A lot of thanks also goes to my reputable instructors during this bootcamp as well as to my fellow learners.
