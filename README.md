## Introduction

* As an undergraduate student at Southern New Hampshire University in the Computer Science program, I have studied numerous topics in the field. From team collaboration using Git, mobile device programming, database implementations, QA testing procedures, to software development life cycles, computer graphics, and secure coding, amongst several others. This breadth of study has given me a wide view of the immense field that is computer science. In the following portfolio, I will demonstrate my abilities to evaluate, develop, review, and enhance several pieces of code targeting three specific categories in the field: software design & engineering, algorithms & data structures, and databases. I also give examples of my skills in working within a team, providing communications in various mediums, as well as demonstrating a security mindset. 

#### Teamwork

* When working in a team environment, I have employed strategies for building collaborative environments that enable diverse audiences to support organizational decision making in the field of computer science by creating an application that benefits the QA department when employed as a firmware/hardware tester. At the time, I had just began teaching myself Python code under the tutelage and encouragement of the department manager. In this QA role, I determined a need for tracking and logging endurance testing being done on various pieces of equipment. Realizing this need, I took it upon myself to plan, design, execute, and test the code. During the application testing phase, I submitted the program to several co-workers to evaluate and give suggestions for improvement. This team collaboration led to the structure of the report being formatted in a way that detailed the critical data that the project managers considered most crucial. The application allowed for logging of test pass and fail attempts, an automatic failure percentage calculator, and document report creation when the testing was completed. Developing this program allowed the team to easily tabulate their findings. It also produced a unified report that was then handed to project managers who could use the data to base decisions concerning product releases and bug evaluations. 

#### Communications

* In the business world, being able to communicate effectively is a crucial skill. Conveying ideas across several mediums allows one to show an understanding of the topic at hand. In this eportfolio, I will demonstrate how I designed, developed, and delivered professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences. 

* For the code review video, I offer an oral explanation of the code artifacts, what their purposes are, any issues and faults in the code, a run-through of the code review checklist that explains if and when the code adheres or not to the checklist, and the planned enhancements to each piece of code. There is also a visual demonstration of the code as I follow along in tandem with my oral review, showcasing each part of the application as it is discussed.

* My written communications are present in this eportfolio, representing my abilities to develop a coherent, consistent, and easy to navigate body of work. Each section of the eportfolio is labelled intuitively and gives the reader quick access to each of the sections for which to review.

#### Computing Solutions

* When it comes to developing software, having a clear understanding of common best practices is crucial. This allows one to easily integrate into a team development environment and maintain cohesive logic. I have designed and evaluated computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices by creating a class for the Animal Shelter project shown below in artifacts #2 and #3. Creating a class that defines the methods made available to the rest of the program. The class is essentially a framework for creating objects. The object’s qualities are defined by each method in the class. Specifically, each method in the Animal Shelter class creates one of the CRUD (Create, Read, Update, Delete) operations that are very commonly used when interfacing with databases. Each of the methods also deals with possible errors by implementing try/except block, which seeks to prevent program crashes in the event of bad or empty data submitted to the method. The class structure itself uses a common schema, for Python in this case, where the __init__ method is called first and always, due to the initialization of class variables. Each time the class is called, the object is created with these initial variables. From there, any of the methods can be called and implemented. 

#### Industry Standards

* Continuing with the same Animal Shelter code, let’s turn our attention to industry standards and practices. I demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals by creating code that uses structure, proper code formatting, and a logical flow of methods. The code begins with the import of the necessary external libraries needed to perform database operations via MongDB and the requisite BSON (Binary JSON) needed to interface with the database.

* Next we see the class declaration which uses Python standard class naming, magic method __init__ which every object creates when the class is called, and method initialization. The __init__ method uses a very common technique in Python of naming the object itself “self”. Each method, if necessary, uses the proper naming standard lowercase letters, and underscores in between distinct words in the name, for example, how_many_items. The CRUD methods employ easy to understand naming as well: create, read, update, delete. Using well-intentioned words for methods makes the code easier to read. This provides value to the teammates reviewing the code or updating the code at a later date as they are not having to guess at what is the purpose of said method. Each method code block follows a very specific format as well. All code within the method is indented 4 spaces. Any code contained within the try/except block is indented an additional 4 spaces. The same indents apply for the code within the if/else statements. This indentation format makes the code more discernible by grouping code that belongs together and creates a separation of concerns, while making the method cohesive. Finally, proper commenting is on display in this code, using the header of the file as the place to read about what the class does, its purpose, and its logic. The comments that follow will apply more specifically to their corresponding code sections. Commenting in this way will once again create an easier experience for code reviews as well as future enhancements to the code, giving the reader easy to understand statements about the different parts of the code.

#### Security Mindset

* A crucial component to software development is ensuring that the code being written takes into account prudent safety measures. I developed a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources by performing several enhancements to the code in my projects. Once again, I will use the Animal Shelter project for this demonstration.

* Looking at each of the methods in the class, there is a try/except block. This code block structure allows for the passing in of data that could cause the application to crash, memory to leak, or nefarious actors to infiltrate. The try section will process the code nested within it. The if data is not None line will pass the value of data only if it meets the criteria of not None. Otherwise, the else statement is run, which will trigger the exception warning. This warning shows an error statement. The except block will only run if the try block is not run. This can be caused by incompatible data being passed into the method when first called. In the event of this happening, an exception is thrown by Python and that error is then assigned to the e variable. Once this exception is thrown, the method is exited and the user will see the error. What this try/except accomplishes is restricting the type of data allowed into the method while also prevented an application crash. When dealing with databases, having security at the forefront of your mind will create a program that protects data, protects the company’s assets and information, while creating a trust between the company and its users. 

#### Summary

* The above assessment showcases the skills that I have learned and acquired throughout my tenure as a Computer Science student at SNHU. Additionally, it provides a clear view of the type and caliber of work of which I am capable. I am confident in my abilities to implement, learn, and employ techniques best coding practices, proper coding techniques, and necessary security safeguards, while keeping present concerns for all stakeholders and end-users. Delving deeper into each subject further, the next section will provide further insight into my capabilities. Each artifact below represents a major necessary skill that is required of all who work in software development: software design/engineering, algorithms and data structures, and databases.

* The Grade Project shows how I have learned to properly structure and design an application that uses standard practices and engineering. The Animal Shelter project is used for the other two artifacts. The first instance will demonstrate my abilities to use proper data structures when confronted with the prospect of repeated code. The list data type reduces code and gives proper structure to the code. For the second usage of the Animal Shelter project, my ability to enhance database operations is shown. By giving the user further options in interfacing with the database, I have shown that I can create an application which offers greater value to both the user and the stakeholders. 

---

## Code Review

* In this section, I will review two code sources to exhibit my abilities to objectively critique code based on a set of prescribed standards in code review. I will provide an overall review of the code's purpose and its functionality. Then, I will review each piece code as it pertains to various aspects, such as code structure, documentation, formatting, etc. And finally, I will provide the identification of, and enhancements that will be performed to improve the code respective of the designated category

* First, the Student Grade project from the Foundations in Application Development course will be reviewed. This code source pertains to the category of **Software Design and Engineering** aspect of code development. 
For the next two sections, the Animal Shelter project from the Client/Server Development course will come under review. This code source will be used for both the **Algorithms and Data Structures** and the **Databases** categories. The only differing sections for this review will come in the last section, the identification and enhancements. 

* Please find the link to the video review [here](https://youtu.be/pMQnrq0jhuo)

<hr>

## Artifact Enhancements

### Artifact \#1 - Software Design & Engineering

* The artifact chosen for this milestone is the **Grade Percentage** project from the IT-145 – Foundations in Application Development course. It was originally created in February of 2019. The application is written in Java. Its purpose is to take in user input of 3 student grades – homework, midterm exam, and final exam – and calculate a final course percentage based on different weighting scales for each of the 3 grades. 

#### Enhancements and Justifications of Artifact Inclusion

* This artifact was chosen as it is good representation of my abilities to write clean and well-formatted code that utilizes an external library, as well as taking user input to then be manipulated and acted upon within the application. Another reason that this artifact was chosen as it demonstrates a logical flow of commands and a separation of concerns. Each sectioned code block is that way for reason. Besides the obvious method separation, the code blocks within each method are spaced from its neighboring code block to make readability much easier and to group code that pertains to the same functionality or purpose.  Lastly, the usage of the Scanner class from the native Java library shows the ability to correctly implement programming language libraries. Referencing the documentation for Java gave me the proper implementation for the Scanner method that was needed to correctly process user input that was needed to execute the calculations within the program. 

* To improve the code, I made the following changes. My first step was to determine which sections of the calculation method would be moved, where it would be moved to, what other components (variables, etc.) should be moved with it. Next, I commented in the code where each item would go. Then, I created the new method. It is a private static method, being private as this method will only be accessed by another method within the program and does not require outside access. Its return type is double, since it will be a decimal number. After that, I moved the calculation method to its newly created method. The arguments passed into the method were there added in the method declaration statement, all passed in as double types. I then noticed that the constants that were declared in the original main method were only being used by the calculation code block. This necessitated me moving them to the new calculation method. These were placed just after the method declaration statement, and just above the calculation code block. The return statement was then added at the end of the method, returning the calculated course percentage. 

#### Course Objectives

* The techniques used to create the application and make the enhancements are consistent with common programming and Java language standards. From library importing, to class usage, method creation and implementation, data type usage, and code formatting, all elements demonstrate the ability to properly execute software design and engineering solutions as well as achieve the specified goals. All logic flows correctly in terms of method placement, arithmetic operations, and user interactions. Using these techniques and skills in computing allows me to provide programming solutions that bring real value to the client and achieve targeted goals. 

* In terms of security, there are a couple portions of the application that do need attention were this to be used outside of my own computer system/network. The user input has no safeguards on it whatsoever. This would need to be restricted to a floating-point data type, i.e., a double. As it stands, the user could input any characters they wished, and the program would not refuse them. Anything outside of a numerical entry would cause either an error to be thrown or also crashing the program. To accomplish this, a simple while loop could be implemented that would test the user’s input as being a double data type. If it is not the prescribed type, the application would continue to prompt the user for proper input. This would also need to be performed for all three user input interactions, meaning this while loop could be another method inside the class, to keep with the concept of D.R.Y.

* Another point of interest in terms of security would be the possibility of exceptions being thrown within the calculation method. In its current iteration, the calculation seems innocuous enough. However, it could pose a problem due to calculation errors. Using a try/catch exception handling code block would help to remedy any issues that could arise here. As an extra precaution, a try/catch exception block could be used around the entirety of the user input section in the main method. 

* Using the prescribe security measures above demonstrates my ability to recognize security and design flaws. Recognizing these potential vulnerabilities displays a security mindset that is crucial to ensuring safe operation for both users and enterprises. By performing these security fixes, I can mitigate security issues and protect all stakeholders from nefarious actors or wasted downtime due to insecure code. 

#### Reflection

* Initially when I pondered how I would enhance this program, what I saw was the calculation code that did make it into the enhancement. It seemed almost too simple that I would just make a new method and move the calculation code into it. I quickly then realized that there were multiple other components that would need to accompany this change. The constants that the calculation uses needed to also be moved to the new method. This meant that the main method would be even further condensed in size, improving legibility. Next, the new method needed the correct return type, which was determined to be a double, since the rest of the types in the calculations were the same data type (floating point numbers). Also needed were the arguments passed into the new method. These needed to match those being used in the calculations, including the proper data type. 

* One of my big takeaways from this enhancement is that something that seems a simple change at first will often contain many other changes that correspond to the intended change. Going forward, it will benefit me to take a broader view of the problem and attempt to reconcile all necessary additions that an enhancement will require for it to be fully realized. 

#### Original Code Pre-Enhancement

```java
package gradeproject;

/*
The following program should compute a student's total course percentage 
based on scores on three items of different weights (%s):

    20% Homeworks (out of 80 points)
    30% Midterm exam (out of 40 points)
    50% Final exam (out of 70 points)

*/

import java.util.Scanner;

public class GradeProject {
   public static void main(String[] args) {
      Scanner scnr = new Scanner(System.in);
      final double HOMEWORK_MAX = 80.0;
      final double MIDTERM_MAX  = 40.0;
      final double FINAL_MAX    = 70.0;
      final double HOMEWORK_WEIGHT = 0.20; 
      final double MIDTERM_WEIGHT  = 0.30;
      final double FINAL_WEIGHT    = 0.50;

      double homeworkScore    = 0.0;
      double midtermScore     = 0.0;
      double finalScore       = 0.0;
      double coursePercentage = 0.0;

      System.out.println("Enter homework score:");
      homeworkScore = scnr.nextDouble();

      System.out.println("Enter midterm exam score:");
      midtermScore = scnr.nextDouble();

      System.out.println("Enter final exam score:");
      finalScore = scnr.nextDouble();

      coursePercentage = ((homeworkScore / HOMEWORK_MAX) * HOMEWORK_WEIGHT)
                       + ((midtermScore / MIDTERM_MAX)    * MIDTERM_WEIGHT)
                       + ((finalScore / FINAL_MAX)          * FINAL_WEIGHT);
      coursePercentage = coursePercentage * 100; // Convert fraction to %

      System.out.print("Your course percentage: ");
      System.out.println(coursePercentage);

      return;
   }
}

```

#### Enhanced Code

```java
package gradeproject;

/*
The following program will compute a student's total course percentage 
based on scores on three items of different weights (%s):

    20% Homeworks (out of 80 points)
    30% Midterm exam (out of 40 points)
    50% Final exam (out of 70 points)

    The user will enter their 3 different grade scores
    Those scores are then weighted by the values listed above
    All 3 weighted scores are added together and then calculated as a percentage

*/

import java.util.Scanner;

public class GradeProject {

   // Method to calculate the weighted score and the course percentage
   private static double gradePercentageCalculation(
                  double homeworkScore, double midtermScore,
                  double finalScore, double percentage) 
   {
      // Declare constants to be used within the calculations
      // These values affect the final calculation
      final double HOMEWORK_MAX    = 80.0;
      final double MIDTERM_MAX     = 40.0;
      final double FINAL_MAX       = 70.0;
      final double HOMEWORK_WEIGHT = 0.20; 
      final double MIDTERM_WEIGHT  = 0.30;
      final double FINAL_WEIGHT    = 0.50;

      // Calculation block - each score type has its own weighting values to be 
      // calculated. The three weighted scores are then added together
      percentage = ((homeworkScore / HOMEWORK_MAX) * HOMEWORK_WEIGHT)
                 + ((midtermScore / MIDTERM_MAX)    * MIDTERM_WEIGHT)
                 + ((finalScore / FINAL_MAX)          * FINAL_WEIGHT);

      // Convert fraction to %           
      percentage = percentage * 100; 

      return percentage;
   }

   // Initialize the Scanner method and the variables for the grades
   public static void main(String[] args) {
      Scanner scnr = new Scanner(System.in);
      double homeworkScore    = 0.0;
      double midtermScore     = 0.0;
      double finalScore       = 0.0;
      double coursePercentage = 0.0;

      // Prompt user for homework score input using Scanner input
      System.out.println("Enter homework score:");
      homeworkScore = scnr.nextDouble();

      // Prompt user for midterm exam score input using Scanner input
      System.out.println("Enter midterm exam score:");
      midtermScore = scnr.nextDouble();

      // Prompt user for final exam score input using Scanner input
      System.out.println("Enter final exam score:");
      finalScore = scnr.nextDouble();

      // Call the calculation method passing the 3 user input variables
      // and the final output variable
      gradePercentageCalculation(homeworkScore, midtermScore, 
                       finalScore, coursePercentage);

      //Print the final grade percentage to the screen
      System.out.print("Your course percentage: ");
      System.out.println(coursePercentage);

      return;
   }
}
```

---

### Artifact \#2 - Algorithms & Data Structures

* The artifact chosen for this milestone is the Animal Shelter project from the CS-340 – Client/Server Development Course. It was originally created in August of 2022. The application is written in Python. The entire project is an application that allows the user to select dogs that fit certain criteria from a database. There were many different aspects of the dogs that the user could then filter with the program: breed, age, sex, location, size, etc. The user had the ability to interact with the database using create, read, update, and delete operations (CRUD). The class that will be updated as part of this artifact is the CRUD operations class. 

#### Enhancements and Justifications of Artifact Inclusion

* This artifact was chosen as it has a great representation of my ability to create a class with multiple methods that also interact with a database. It gives me the opportunity to use a data structure to reduce some of the excess code that is repeated. It is also a great candidate to display the readability of the code that I write, in terms of formatting, clear code sections, and informative comments. In particular, to show my skills in data structures, I’ve implemented a list data type that will be accessed in each of the four CRUD methods. This list contains the string statements that are displayed to the user when there is an exception thrown by insufficient data being passed to the method. 
* To improve the code, the following changes were made. Initially, FIXME comments were added to the different parts of the code that were going to be enhanced. These included the new list section, debug statements that needed removing. the header section, as well as a few spots in the method where clarity was needed. Then the detailed comments were added to those sections. There were also a few comments that needed to be indented to line up with there respective method declaration lines. 
Next, the list was created. This was placed directly underneath the class declaration line. Each statement was taken from their original positions within the methods and placed within the list. There are two statements in total for the four methods. Next up, the exception statements within each method were replaced with the call to the new lists, using the correct index number for each. Then, more comments were added to the header to provide more clarity of the program’s intention and functionality. Finally, the debug statements were removed from their positions, as these are no longer needed.

#### Course Objectives

* For this enhancement, the course objective was to solve a given problem by using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices. I accomplished this by making good use of a data structure type that is extremely useful in programming, the list. This array type allows for grouping multiple items together into comma separated values. These different items in the list are then accessed via their index (or position) within the list by calling the list name and include the desired index. The list I created contains two different strings. These strings were originally inside of each CRUD method as an exception statement. Now inside of each statement exists the call to the list with either a 0 or 1 as the index argument. One of the benefits of this is the reduction of code, creating a smaller code base. If more methods were created in this class, the list could easily be implemented there, or even modified to include additional statements that can then be used as needed. 
* Designing, developing, and delivering professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts is a necessary skill in this day and age. The ability to deliver a well written communication about the code is also being presented here. By adding pertinent information to this narrative, the reader can clearly determine what changes were made to the code, what the intentions were, what the new enhancements offer in terms of increased programming abilities, and my ability to utilize the skills learned in the computer science courses. Looking at the header comments in the code, there is a clear description of the application’s purpose and its objective. There are details concerning the CRUD functionality, the type of database being used, MongoDB, and how the authorization works. 

#### Reflection

* One of the things that I learned while modifying this artifact is that readability is a very important component of well-written code. The formatting and sectioning of different parts of the code make it much more manageable in terms of finding particular items of interest. For instance, the different exceptions statements that I would be moving into the list easily stood out on the screen as they were each in the same position within their respective methods. Another thing I learned was that the placement of the list needs to be specific. It must be initialized before any piece of code that calls that list. If it’s not been created by the time the program makes its way to the list call, an error will occur. For this reason, the list is position before all of the CRUD method calls which use the list. 
* As far as challenges while enhancing this artifact, there was nothing major that blocked my achievement of the modification. A list is a very common data type, and its implementation was relatively straightforward. I did need to reference the Python documentation to make sure the correct brackets were used in the list calls, the non-curly brackets []. I did have to determine where to place the line break within the list, as the exceptions statements are of decent length. Having them all on a single line of code would have made that code line extend much further out on the page. This would not affect functionality in any way; it would just be looked at as incorrect code formatting.

#### Original Code Pre-Enhancement (used in both artifact #2 & #3)

```python
from pymongo import MongoClient
from bson.objectid import ObjectId

class AnimalShelters(object):
    """ CRUD operations for Animal collection in MongoDB """

    def __init__(self, username, password):
        # Initializing the MongoClient. This helps to 
        # access the MongoDB databases and collections. 
        self.username = username
        self.password = password
        self.client = MongoClient('mongodb://%s:%s@localhost:53184/AAC' % (username, password))
        self.database = self.client['AAC']

# Create method. Uses the insert_one() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def create(self, data) -> bool:
        try:
            if data is not None:
                self.database.animals.insert(data)  # data should be dictionary
                print("True")
                return True
            else:
                raise Exception("Nothing to save, because data parameter is empty")
                return False
        except Exception as e:
            print(e)

# Read method. Uses the find() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def read(self, key_val) -> set:
        try:
            if key_val is not None:                
                data = self.database.animals.find(key_val, {"_id": False})
            else:
                data = Exception("Nothing to save, because data parameter is empty")
            return data
        except Exception as e:
            print(e)
            
            
# Update method. Uses the updateOne() Mongo method    
# Pass in key/value pairs in JSON format. Requires two arguments
    def update(self, data, changes):
        try:
            if (data is not None) and (changes is not None):
                setChange = {"$set":changes}
                self.database.animals.update_one(data, setChange)
                updated_doc = self.database.animals.find(changes)
                print('Update Successful!')
                return updated_doc
            else:
                data = Exception("Nothing to save, because data parameter is empty")
                return data
        except Exception as e:
            print(e)
            
# Delete method. Uses the deleteOne() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def delete(self, data):
        try:
            if data is not None:
                self.database.animals.delete_one(data)
                print("Delete Successful!")
                deleted_doc = self.database.animals.find(data)
                return deleted_doc
            else:
                data = Exception("Nothing to delete, because data parameter is empty")
                return data
        except Exception as e:
            print(e)
                
```

#### Enhanced Code

```python
"""
The purpose of this class is to provide CRUD functionality to the application
Each of the CRUD operations is contained within its own class method
The init method contains the MongoDB address as well as defines the database

MongoDB is the database used
A username and password is required for authorization to use the database
user/pass is fed from the file calling this class
"""

# Library imports
# MongoClient enables work with MongoDB
from pymongo import MongoClient
from bson.objectid import ObjectId

class AnimalShelters(object):
    """ CRUD operations for Animal collection in MongoDB """

    # List containing exceptions text
    exceptions_list = ["Nothing to save, because data parameter is empty",
                       "Nothing to delete, because data parameter is empty"]
    
    # Init method, declaring class variables                       
    def __init__(self, username, password):
        # Initializing the MongoClient. This helps to 
        # access the MongoDB databases and collections. 
        self.username = username
        self.password = password
        self.client = MongoClient('mongodb://%s:%s@localhost:53184/AAC' % (username, password))
        self.database = self.client['AAC']

    # Create method. Uses the insert() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'data' will be dict type
    def create(self, data) -> bool:
        try:
            if data is not None:
                self.database.animals.insert(data)  
                return True
            else:
                raise Exception(exceptions_list[0])
                return False
        except Exception as e:
            print(e)

    # Read method. Uses the find() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'key_val' will be dict type
    def read(self, key_val) -> set:
        try:
            if key_val is not None:                
                data = self.database.animals.find(key_val, {"_id": False})
            else:
                data = Exception(exceptions_list[0])
            return data
        except Exception as e:
            print(e)
            
    # Update method. Uses the updateOne() Mongo method    
    # Pass in key/value pairs in JSON format. Requires two arguments
    # 'data' and 'changes' will be dict types
    def update(self, data, changes):
        try:
            if (data is not None) and (changes is not None):
                setChange = {"$set":changes}
                self.database.animals.update_one(data, setChange)
                updated_doc = self.database.animals.find(changes)
                return updated_doc
            else:
                data = Exception(exceptions_list[0])
                return data
        except Exception as e:
            print(e)
            
    # Delete method. Uses the deleteOne() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'data' will be dict type
    def delete(self, data):
        try:
            if data is not None:
                self.database.animals.delete_one(data)
                deleted_doc = self.database.animals.find(data)
                return deleted_doc
            else:
                data = Exception(exceptions_list[1])
                return data
        except Exception as e:
            print(e)
```

---

### Artifact \#3 - Databases

* The artifact chosen for this milestone is the Animal Shelter project from the CS-340 – Client/Server Development Course. It was originally created in August of 2022. The application is written in Python. The entire project is an application that allows the user to select dogs that fit certain criteria from a database. There were many different aspects of the dogs that the user could then filter with the program: breed, age, sex, location, size, etc. The user had the ability to interact with the database using create, read, update, and delete operations (CRUD). The class that will be updated as part of this artifact is the CRUD operations class. 

#### Enhancements and Justifications of Artifact Inclusion

* This artifact was chosen as a good example of my work with databases and creating classes that perform a specific grouping of functions. In this case, the class offers Create, Read, Update, and Destroy (CRUD, a very common methodology for interacting with databases) methods. As you can see in the class code, each method is created using the same structural format. A try/except block is used to mitigate any possible exception errors that may arise from either faulty input, or other computational errors. Inside each of those blocks, an if/else statement is used to compare the passed arguments to a value of None. This comparison serves as a guard against empty values being passed from the code calling this class. When an acceptable argument is passed to said method, it is processed according to each method’s needs: read, delete, etc. After performing the necessary operation(s), the returned data is sent back to the calling code for use by the user. These specific components above show my abilities to properly access and interact with databases. 

* To improve the code, the following changes were made:
First, FIXME comments were added to the code in the spots with planned enhancements. These were in the read method as well as just underneath the __init__ method. This serves as a guide and reminder of where I need to edit the code. Next, I created the call to the new method inside the read method. This method call is placed just under the read method’s declaration line. This is necessary as the data returned to this new method will be used later in the read method. Then, I created the how_many_items method. This was placed just under the __init__ method. A new line was created in this method to prompt the user for how many items they would like returned. The return statement was placed just after that to complete the method. The return statement was passed the variable containing the user’s number of items input from the previous line. I needed to add the argument to this new method, as a value needs to be returned. This argument then becomes the variable prompting for user input. I then added the argument variable in the call to the new method, back in the read method. Realizing that this new variable was not yet initialized, I created a line just above the method call initializing the variable with a value of zero. To implement this into the read method, a new MongoDB method was added to the .find() line. Using the .limit(#) method, the argument passed into it is the variable containing the returned value from the new method created for this enhancement. To complete the enhancement, the original FIXME comments were removed from the code and explanatory comments for the new changes were added. 

#### Course Objectives

* For this enhancement, the objective was to demonstrate my ability to work with databases and improve the code that demonstrates this skill. I accomplished this skill by identifying a potential problem in the number of items returned by the database. Depending on the database, a user could receive numerous returned items (hundreds, thousands ?) which could overwhelm them. It could also cause the computer system to ‘hang’ when waiting an excessive number of items. To mitigate these two issues, a new option was offered with this enhancement. The user could restrict the returned number of items. This lessens the strain on the database system and provides a cleaner, more usable set of data for which the user can observe. This enhancement also demonstrates my ability to employ strategies for building collaborative environments that enable diverse audiences to support organizational decision making in the computer science field.
* The issue of excessive data being returned by the database causes users to wait for processing of the database to complete. This wait time is inefficient and produces no positive outcome in terms of productivity for the team. By creating a cap on the number of returned items, this enhancement gives each team member the ability to decrease wait times and improve workflow both for the user and the machines running the applications, increasing efficiency and productivity.

#### Reflection

* As I worked through this enhancement, I was reminded of the differing types of conventions that programming languages use. Python is like any other language in that it has similar naming conventions while also possessing differing ones. Consulting Python’s programming standards, I was able to properly format the method names, the variable names, as well as the method construction format. Another Python special format that I needed to ascertain was how to prompt the user for input. Here, I consulted the Python documentation to procure the correct implementation. Lastly, I had to consult the MongoDB documentation to determine which method was needed to restrict the returned items. 
* As for what I learned in this exercise, one overarching theme was programming language standards. With all the different languages available to use, it is imperative that reading the documentation and using language-specific formatting standards is enacted. This ensures readability for other developers as they will for sure be reading my code in the future. Adhering to standards makes for a more cohesive and more productive learning and working environment. Some companies will also enact their own standards, making this practice even more pertinent to developer cohesiveness. 


#### Original Code Pre-Enhancement (used in both artifact #2 & #3)

```python
from pymongo import MongoClient
from bson.objectid import ObjectId

class AnimalShelters(object):
    """ CRUD operations for Animal collection in MongoDB """

    def __init__(self, username, password):
        # Initializing the MongoClient. This helps to 
        # access the MongoDB databases and collections. 
        self.username = username
        self.password = password
        self.client = MongoClient('mongodb://%s:%s@localhost:53184/AAC' % (username, password))
        self.database = self.client['AAC']

# Create method. Uses the insert_one() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def create(self, data) -> bool:
        try:
            if data is not None:
                self.database.animals.insert(data)  # data should be dictionary
                print("True")
                return True
            else:
                raise Exception("Nothing to save, because data parameter is empty")
                return False
        except Exception as e:
            print(e)

# Read method. Uses the find() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def read(self, key_val) -> set:
        try:
            if key_val is not None:                
                data = self.database.animals.find(key_val, {"_id": False})
            else:
                data = Exception("Nothing to save, because data parameter is empty")
            return data
        except Exception as e:
            print(e)
            
            
# Update method. Uses the updateOne() Mongo method    
# Pass in key/value pairs in JSON format. Requires two arguments
    def update(self, data, changes):
        try:
            if (data is not None) and (changes is not None):
                setChange = {"$set":changes}
                self.database.animals.update_one(data, setChange)
                updated_doc = self.database.animals.find(changes)
                print('Update Successful!')
                return updated_doc
            else:
                data = Exception("Nothing to save, because data parameter is empty")
                return data
        except Exception as e:
            print(e)
            
# Delete method. Uses the deleteOne() Mongo method
# Pass in key/value pairs in JSON format. Requires one argument
    def delete(self, data):
        try:
            if data is not None:
                self.database.animals.delete_one(data)
                print("Delete Successful!")
                deleted_doc = self.database.animals.find(data)
                return deleted_doc
            else:
                data = Exception("Nothing to delete, because data parameter is empty")
                return data
        except Exception as e:
            print(e)
                
```

#### Enhanced Code

```python

"""
The purpose of this class is to provide CRUD functionality to the application
Each of the CRUD operations is contained within its own class method
The init method contains the MongoDB address as well as defines the database
A method to accept user input restricts the number of returned items in the read method. 


MongoDB is the database used
A username and password is required for authorization to use the database
user/pass is fed from the file calling this class
"""

# Library imports
# MongoClient enables work with MongoDB
from pymongo import MongoClient
from bson.objectid import ObjectId

class AnimalShelters(object):
    """ CRUD operations for Animal collection in MongoDB """

    # List containing exceptions text
    exceptions_list = ["Nothing to save, because data parameter is empty",
                       "Nothing to delete, because data parameter is empty"]
    
    # Init method, declaring class variables                       
    def __init__(self, username, password):
        # Initializing the MongoClient. This helps to 
        # access the MongoDB databases and collections. 
        self.username = username
        self.password = password
        self.client = MongoClient('mongodb://%s:%s@localhost:53184/AAC' % (username, password))
        self.database = self.client['AAC']

    # Prompt user for input of how many items they desire to be returned in read method
    # Return value is a num type
    def how_many_items(self, numItems):
        numItems = print("How many options would you like returned? ")
        return numItems

    # Create method. Uses the insert() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'data' will be dict type
    def create(self, data) -> bool:
        try:
            if data is not None:
                self.database.animals.insert(data)  
                return True
            else:
                raise Exception(exceptions_list[0])
                return False
        except Exception as e:
            print(e)

    # Method to prompt user for number of returned items
    # The variable declaration is simply for the object passed to the method call
    # Read method. Uses the find() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'key_val' will be dict type
    def read(self, key_val) -> set:
        numItems = 0
        how_many_items(numItems)
        try:
            if key_val is not None:                
                data = self.database.animals.find(key_val, {"_id": False}).limit(numItems)
            else:
                data = Exception(exceptions_list[0])
            return data
        except Exception as e:
            print(e)
            
    # Update method. Uses the updateOne() Mongo method    
    # Pass in key/value pairs in JSON format. Requires two arguments
    # 'data' and 'changes' will be dict types
    def update(self, data, changes):
        try:
            if (data is not None) and (changes is not None):
                setChange = {"$set":changes}
                self.database.animals.update_one(data, setChange)
                updated_doc = self.database.animals.find(changes)
                return updated_doc
            else:
                data = Exception(exceptions_list[0])
                return data
        except Exception as e:
            print(e)
            
    # Delete method. Uses the deleteOne() Mongo method
    # Pass in key/value pairs in JSON format. Requires one argument
    # 'data' will be dict type
    def delete(self, data):
        try:
            if data is not None:
                self.database.animals.delete_one(data)
                deleted_doc = self.database.animals.find(data)
                return deleted_doc
            else:
                data = Exception(exceptions_list[1])
                return data
        except Exception as e:
            print(e)
```      
