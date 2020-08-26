## **Rest-api-Assignment**

This repository is to learn how to design,develop and test a Rest api web service

The Assignment is to design, develop and test a Rest api web service for an Online Bookstore.

Scenario: Student Records

The main resource are students. A Student object has attributes such as unique id, a name, an address, a semester , a dregree program and a number of courses

## **APIs for Students in School**

1: Creating  A record : Create a new student 
•	Request Header
 **CREATE****:**  https://www.abcschool.com/student/createStudent

    {
             ("id", 1);
    		 ("name", "Omer");
    		 ("gender", "M");
    		 ("address", "Australia");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "6");
    }

•	Response Header
HTTP response code – 201 Created

    {
             ("id", 1);
    		 ("name", "Omer");
    		 ("gender", "M");
    		 ("address", "Australia");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "6");
    }


2: Getting  A record : Get a student by giving student id
•	Request Header
**GET** **:**  https://www.abcschool.com/student/1

    {
             ("id", 1);
    		 ("name", "Omer");
    		 ("gender", "M");
    		 ("address", "Australia");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "6");
    }

•	Response Header
HTTP response code – 200 OK

    {
             ("id", 1);
    		 ("name", "Omer");
    		 ("gender", "M");
    		 ("address", "Australia");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "6");
    }


3: Getting all the records: Get all the records of all the semesters in a student table
•	Request Header
****GET**:** https://www.abcschool.com/student 

•	Response Header
HTTP response code – 200 OK

    [
    {
             ("id", 1);
    		 ("name", "Omer");
    		 ("gender", "M");
    		 ("address", "Australia");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "6");
    }
    {
             ("id", 2);
    		 ("name", "Hamna");
    		 ("gender", "F");
    		 ("address", "United STATES");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "5");
    }
    {
    
                  ("id", 3);
    		 ("name", "SAJINA");
    		 ("gender", "F");
    		 ("address", "AUSTRALIA");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "8");
    
    
    }
    ]

4: Updating A record  Updating a student semester by giving student id
•	Request Header
**UPDATE:** https://www.abcschool.com/student/2

    {
    
             ("id", 2);
    		 ("name", "Hamna");
    		 ("gender", "F");
    		 ("address", "United STATES");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "8");
    }

•	Response Header
HTTP response code – 201 Created

    {
    
             ("id", 2);
    		 ("name", "Hamna");
    		 ("gender", "F");
    		 ("address", "United STATES");
    		 ("degreeProgram", "CS");
    		 ("semester", "8");
    		 ("numberOfCourses", "8");
    }


5: Deleting a record : Delete the Address by giving the student id
•	Request Header

**DELETE:** https://www.abcschool.com/student/1

•	Response Header
HTTP response code – 200 OK / 204 No Content





