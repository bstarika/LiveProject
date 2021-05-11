# Live Project
## Introduction:
I was able to gain real-world experience during the Live Project at The Tech Academy. We worked on a MVC Web Application for a Theatre, utilizing both front / [back-end development](#back-end-development) and agile methodologies. It was a two week sprint, and during that time I was able to complete five stories and participate in daily standups - including a code retrospective. Our team used Azure Devops for the project, Visual Studio as an IDE, and Slack for communication. Thanks to the final project, I now can confidently navigate Visual Studio and understand the workflow for clean Version Control. I know how to create branches, update the local master branch, push code, create pull requests, resolve merge conflicts, and so much more.
## Back-End Development:
[Helper Method](#helper-method), [Entity Model and CRUD Pages](#entity-model-and-crud-functionality), [Creating User](#creating-user)
### Helper Method
My first story consisted of writing a helper function that was used to limit the number of characters that were displayed using ellipses. I created a static method in a C# class that took in a string and an integer. The string was the content that we were trying to truncate and the integer represented how many characters were allowed before cutting off the string and adding ellipses ( . . . ). I had to test my method in the Index page to ensure it worked before submitting. 
![alt text](https://github.com/bstarika/LiveProject/blob/main/HelperMethod.jpg?raw=true)
Testing the helper method by setting the int limit to 50.
![alt text](https://github.com/bstarika/LiveProject/blob/main/TestingHelperMethod.jpg?raw=true)
### Entity Model and CRUD Functionality
There were 3 parts to this story: Create a model for CastMember, an enum for positions, and CRUD functionality. <br>
Below I created an Entity Model for the CastMember class so that cast members could be saved to the database. The "?" indicates the property is nullable. I also created a Position Enum for the Main Role.
![alt text](https://github.com/bstarika/LiveProject/blob/main/EntityModelandEnum.jpg?raw=true) <br>
Scaffolded Cast Member controller with CRUD functionality - a code generation technique to allow for database access.
![alt text](https://github.com/bstarika/LiveProject/blob/main/CRUDScaffolding.jpg?raw=true) <br>
Migrated changes and added table by adding DbSet and using the "update-database" command with NuGet's Package Manager Console.
![alt text](https://github.com/bstarika/LiveProject/blob/main/UpdateDatabase.jpg?raw=true)
### Creating User 
In this story, I was instructed to create an Application User for a Cast Director. This user was an admin in my assigned section (Productions). I created a new model for the Cast Director that extends from the Application User. I didn't add the Cast Director to the ApplicationDbContext as they wanted a TPH, or a Table Per Hierarchy structure where there were multiple classes in one table. I then added two int properties to show the number of people that the Cast Director has hired and fired.
![alt text](https://github.com/bstarika/LiveProject/blob/main/CastDirectorUser.jpg?raw=true)
### Seed Method
To test out the above Cast Director class, I had to create a seed method. I created an instance of the Cast Director to seed the database, where it is saved to the database before the page is loaded for testing purposes. I wrote the method in the Cast Director class and called the method in the Configuration Seed method. As a result, the method seeded one Cast Director into the database. I had to also create a user role and assign it to the Cast Director being seeded. I then set the properties to my choosing, and ensured to add a password. 
![alt text](https://github.com/bstarika/LiveProject/blob/main/CastDirectorSeedMethod.jpg?raw=true)
## Front-End Development:
## Agile Methodologies:
