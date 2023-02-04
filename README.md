## Code Review

* In this section, I will review two code sources to exhibit my abilities to objectively critique code based on a set of prescribed standards in code review. I will provide an overall review of the code's purpose and its functionality. Then, I will review each piece code as it pertains to various aspects, such as code structure, documentation, formatting, etc. And finally, I will provide the identification of, and enhancements that will be performed to improve the code respective of the designated category

* First, the Student Grade project from the Foundations in Application Development course will be reviewed. This code source pertains to the category of **Software Design and Engineering** aspect of code development. 
For the next two sections, the Animal Shelter project from the Client/Server Development course will come under review. This code source will be used for both the **Algorithms and Data Structures** and the **Databases** categories. The only differing sections for this review will come in the last section, the identification and enhancements. 

* Please find the link to the video review [here](https://youtu.be/pMQnrq0jhuo)

<hr>

## Artifact Enhancements

### Artifact \#1 - Software Design & Engineering

The artifact chosen for this milestone is the **Grade Percentage** project from the IT-145 – Foundations in Application Development course. It was originally created in February of 2019. The application is written in Java. Its purpose is to take in user input of 3 student grades – homework, midterm exam, and final exam – and calculate a final course percentage based on different weighting scales for each of the 3 grades. 

#### Enhancements and Justifications of Artifact Inclusion

This artifact was chosen as it is good representation of my abilities to write clean and well-formatted code that utilizes an external library, as well as taking user input to then be manipulated and acted upon within the application. Another reason that this artifact was chosen as it demonstrates a logical flow of commands and a separation of concerns. Each sectioned code block is that way for reason. Besides the obvious method separation, the code blocks within each method are spaced from its neighboring code block to make readability much easier and to group code that pertains to the same functionality or purpose.  Lastly, the usage of the Scanner class from the native Java library shows the ability to correctly implement programming language libraries. Referencing the documentation for Java gave me the proper implementation for the Scanner method that was needed to correctly process user input that was needed to execute the calculations within the program. 

To improve the code, I made the following changes. My first step was to determine which sections of the calculation method would be moved, where it would be moved to, what other components (variables, etc.) should be moved with it. Next, I commented in the code where each item would go. Then, I created the new method. It is a private static method, being private as this method will only be accessed by another method within the program and does not require outside access. Its return type is double, since it will be a decimal number. After that, I moved the calculation method to its newly created method. The arguments passed into the method were there added in the method declaration statement, all passed in as double types. I then noticed that the constants that were declared in the original main method were only being used by the calculation code block. This necessitated me moving them to the new calculation method. These were placed just after the method declaration statement, and just above the calculation code block. The return statement was then added at the end of the method, returning the calculated course percentage. 

#### Course Objectives

Course Objectives
The techniques used to create the application and make the enhancements are consistent with common programming and Java language standards. From library importing, to class usage, method creation and implementation, data type usage, and code formatting, all elements demonstrate the ability to properly execute software design and engineering solutions as well as achieve the specified goals. All logic flows correctly in terms of method placement, arithmetic operations, and user interactions. Using these techniques and skills in computing allows me to provide programming solutions that bring real value to the client and achieve targeted goals. 

In terms of security, there are a couple portions of the application that do need attention were this to be used outside of my own computer system/network. The user input has no safeguards on it whatsoever. This would need to be restricted to a floating-point data type, i.e., a double. As it stands, the user could input any characters they wished, and the program would not refuse them. Anything outside of a numerical entry would cause either an error to be thrown or also crashing the program. To accomplish this, a simple while loop could be implemented that would test the user’s input as being a double data type. If it is not the prescribed type, the application would continue to prompt the user for proper input. This would also need to be performed for all three user input interactions, meaning this while loop could be another method inside the class, to keep with the concept of D.R.Y.

Another point of interest in terms of security would be the possibility of exceptions being thrown within the calculation method. In its current iteration, the calculation seems innocuous enough. However, it could pose a problem due to calculation errors. Using a try/catch exception handling code block would help to remedy any issues that could arise here. As an extra precaution, a try/catch exception block could be used around the entirety of the user input section in the main method. 

Using the prescribe security measures above demonstrates my ability to recognize security and design flaws. Recognizing these potential vulnerabilities displays a security mindset that is crucial to ensuring safe operation for both users and enterprises. By performing these security fixes, I can mitigate security issues and protect all stakeholders from nefarious actors or wasted downtime due to insecure code. 

#### Reflection

Initially when I pondered how I would enhance this program, what I saw was the calculation code that did make it into the enhancement. It seemed almost too simple that I would just make a new method and move the calculation code into it. I quickly then realized that there were multiple other components that would need to accompany this change. The constants that the calculation uses needed to also be moved to the new method. This meant that the main method would be even further condensed in size, improving legibility. Next, the new method needed the correct return type, which was determined to be a double, since the rest of the types in the calculations were the same data type (floating point numbers). Also needed were the arguments passed into the new method. These needed to match those being used in the calculations, including the proper data type. 

One of my big takeaways from this enhancement is that something that seems a simple change at first will often contain many other changes that correspond to the intended change. Going forward, it will benefit me to take a broader view of the problem and attempt to reconcile all necessary additions that an enhancement will require for it to be fully realized. 

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

