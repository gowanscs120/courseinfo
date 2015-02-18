# Homework 1

## Goals

* Become familiar with the lab environment.
* Get used to Eclipse, the development environment you will be using for this class.
* Introduce you to a basic Java application.
* Introduce you to testing your code.
* Learn how to submit assignments on moodle.

## Login

The computer lab is in H-245. We will be using Windows on the iMac computers. As soon as you walk into the lab make a u-turn and you will see the iMacs.

Pick a computer and login using your pipeline credentials. If you have any problems talk to me or the LTA.

## Eclipse

1. Start eclipse. Double-click the purple globe icon with the label cs120 under it.
1. Create a new Java Project. Click File -> New -> Java Project.
1. In the "Project name:" text box your project name that follows the form `{First Initial}{Middle Initial}{Last Name}-hw1`.
My name is Arnold David Gowans so my project name would be: `adgowans-hw1` which must be all lower case. **This format is required and assignments will not be graded without this format.
**
1. Open your project. Double click the folder with your project name on the left.
1. Create a new package. Right click the `src` folder and select New -> package. Copy `edu.sbcc.hw1` into the "Name:" field.
1. Create a new class. Right click the `edu.sbcc.hw1` package on the left and select New -> Class.  In the "Name:" field type `Car`. Click "Finish".
1. In the file that opened replace all the contents with the following:

  ```java
  package edu.sbcc.hw1;

  public class Car {

  	// ***** Behaviors (Methods) *****
  	public void accelerate(Integer amountToIncreaseBy) {
  		speed = speed + amountToIncreaseBy;
  	}

  	public Integer getSpeed() {
  		return speed;
  	}

  	public void decelerate(Integer amountToDecreaseBy) {
  		// TODO YOUR CODE GOES HERE
  	}

  	// ***** Attributes (Instance variables) *****
  	private Integer speed = 0;

  }
  ```
1. On the keyboard press: `Ctrl + Shift + F`. This will auto format your code. Get in the habit of using it regularly.
1. Create another new class as above but this time named `Main`.
1. In the file that opened replace all the contents with the following:

  ```java
  package edu.sbcc.hw1;

  public class Main {

  	public static void main(String[] args) {
      // SETUP DO NOT EDIT
  		Car myEclipse = new Car();
  		System.out.println("Current speed of my Eclipse: "
  				+ myEclipse.getSpeed());
  		System.out.println("Increasing Speed by 5");
  		myEclipse.accelerate(5);
  		System.out.println("Current speed of my Eclipse: "
  				+ myEclipse.getSpeed());

  		Car myBMW = new Car();
  		// TODO YOUR CODE GOES HERE

  		// TESTS - DO NOT EDIT
  		System.out.println();
  		System.out.println("TESTS");
  		System.out.println("-----");
  		System.out.println("TEST 1 -> Expected Value: " + 5 + " Actual Value: "
  				+ myEclipse.getSpeed());
  		System.out.println("TEST 2 -> Expected Value: " + 20 + " Actual Value: "
  				+ myBMW.getSpeed());
  		myBMW.decelerate(5);
  		System.out.println("TEST 3 -> Expected Value: " + 15 + " Actual Value: "
  				+ myBMW.getSpeed());
  		myBMW.decelerate(0);
  		System.out.println("TEST 4 -> Expected Value: " + 15 + " Actual Value: "
  				+ myBMW.getSpeed());
  		myBMW.decelerate(2);
  		System.out.println("TEST 5 -> Expected Value: " + 13 + " Actual Value: "
  				+ myBMW.getSpeed());
  		System.out.println("Each test is worth 1 points for a total of 5 Points.");
  	}
  }
  ```
11. Run the application. Click the white arrow in the green circle to run your application.

12. You should see the output of the application in the "Console" window.

## Your Assignment

Here is the UML Class Diagram for this project:

![UML Class Diagram](hw1UML.png)

Edit the code in both the Car.java file and Main.java file wherever you see a **TODO** such that all the tests pass (Expected value = Actual value) when you run the application.

## Turn-in

Zip up your entire project for submission:
  * Right click your project folder in eclipse (adgowans-hw1).
  * Click on `export...`
  * Type `archive`
  * Double click on `Archive File`
  * Click on `Browse...`
  * Name the file the same as the project (adgowans-hw1)
  * Choose a location that you will remember like Desktop or Documents.
  * Click `Save`
  * Review the filename and location is as you intend.
  * Click `Finish`

Submit your assignment to moodle.
  * Open a web browser.
  * Navigate to [pipeline](http://pipeline.sbcc.edu).
  * Login with your pipeline credentials.
  * Click on class tab.
  * Click on "Moodle 2" on the right.
  * Click on the CS - 120 link.
  * This is your gateway to the class and where all your assignments will be submitted.
  **BECOME FAMILIAR WITH IT!**
  * Click on Homework 1, and use the submission area to upload your zipped project and submit your assignment.

## Congratulations on completing your first Java application and homework!!!
