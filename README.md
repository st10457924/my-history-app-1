# my-history-app-1
1.Purpose
A history app functions as the historical events' entrance gate to living people through historical timelines, specific events that happened within historical time periods. History and art museums are the locations at which students can obtain a clear picture of history through this app. This can be made possible by means of interactive features, guest lectures and different kinds of artistic activities. Although apps have the potential to engage a wide range of audience, like history lovers, teachers or simple learners, the applications have a double role of viewing the events which has replaced the usage of boring books alongside easy narration. these features do matter but also except difference, people can change their knowledge intake level into an easy or difficult one to base on their wish.

2.Design Considerations
 

Intuitive design:
The user will be able to navigate through the application very easily, it just requires a little bit of patience.
Content Prioritisation:
I've used an ancient which is perfect for My History App to attract the user's attention
Legible Text Content:
The text is large enough for the user to see and the font is easy to read
Make Interface Elements Clearly Visible:
The user will be able to see all components on the screen whether they are in the dark or light
Hand Position Control:
The controls are not too close to each other so you can freely use your thumb or even both thumbs 
Images:
I have chosen historical photographs that shows the content and provide visual context to the historical narratives 

3.GitHub and GitHub Actions:
https://github.com/st10457924/MyHistoryApp1
1. Create a New GitHub Repository:
Go to the GitHub website (https://github.com/) and sign in to your account.
Click on the "+" icon in the top right corner and select "New repository".
Give your repository a name (st10457924 Njabulo), add a description (use IMAD5112 Assignment 1) and choose public.
Click on the "Create repository" button.
2. Initialize the Repository with a README File:
After creating the repository, you'll see an option to "Initialize this repository with a README". Check this option to create a README file.
Click on the "Create repository" button to finalize the creation of the repository.
3. Commit and Push Your Project Files to the GitHub Repository:
In Android Studio, go to VCS (Version Control System) -> Import into Version Control -> Share Project on GitHub.
Log in to your GitHub account if prompted and select the repository you created earlier.
Click on the "Share" button to push your project files to the GitHub repository.
4. Regularly Commit and Push Your Code as You Make Progress:
After the initial push, continue making changes to your project in Android Studio.
Whenever you make significant progress or changes, commit your changes locally in Android Studio using VCS -> Commit Changes.
Once committed, push your changes to the GitHub repository using VCS -> Git -> Push.
 
Testing and Automated Testing:
1. Conduct Manual Testing:
Manually test your app to ensure it functions seamlessly and offers an enjoyable educational experience for learners.
To test various features and user interactions do the following:
1. Create a New Test Class:
In your Android project, navigate to the test's directory (or create it if it doesn't exist).
Create a new Kotlin file for your test class. Name it appropriately to indicate what component or functionality you are testing.
2. Write Test Methods:
 
Inside the test class, write test methods like the example below.
3. Use assertions to verify the expected behavior of your code.
4. Run the Tests:
Run the tests using the testing framework's tools provided by Android Studio or through the command line.
Sample of a test class using JUnit:
 
import org.junit.Assert.*
import org.junit.Test
 
class MyUnitTest {
 
   @Test
   fun testWhenStatement() {
       // Test case for a when statement
       val result = when (25) {
           50 -> "Michael Jackson, famous for sing pop music and died at the age   of 50''
           41 -> "Kobe Bryant, famous for being the 18-time All-Star who won five NBA championships and died at the age of 41"
           40 -> "Paul Walker, famous for his role in the hit film Varsity Blues in 1999, and died at the age of 40"
           else -> "Nobody famous known to me died at this age"
       }
       
       assertEquals("Nobody famous known to me died at this age", result)
     }
 
   }
2. GitHub Actions for Automated Testing:
Set up GitHub Actions to automatically run tests and build your code whenever changes are pushed to the repository.
Create a GitHub Actions workflow (.github/workflows/tests.yml) to run tests automatically on every push:
Create a .github/workflows directory in your project repository.
Inside this directory, create YAML files defining your GitHub Actions workflows for testing and building.
Sample GitHub Actions Workflow for Testing (tests.yml):
name: Run Tests
 
on: [push]
 
jobs:
 test:
   runs-on: ubuntu-latest
 
   steps:
     - name: Set up JDK
       uses: actions/setup-java@v2
       with:
         distribution: 'adopt'
         java-version: '11'
 
     - name: Check out code
       uses: actions/checkout@v2
 
     - name: Build and test
       run: ./gradlew test
 
Set Up Automated Build:
Create a GitHub Actions workflow (.github/workflows/build.yml) to build the APK automatically on every push.
Sample GitHub Actions Workflow for Building (build.yml):
name: Build APK
 
on: [push]
 
jobs:
 build:
   runs-on: ubuntu-latest
 
   steps:
     - name: Set up JDK
       uses: actions/setup-java@v2
       with:
         distribution: 'adopt'
         java-version: '11'
 
     - name: Check out code
       uses: actions/checkout@v2
 
     - name: Build APK
       run: ./gradlew assembleDebug
Test your workflows by pushing changes to your repository and observing the actions running in the "Actions" tab on GitHub.

Link To YouTube Video:
https://eur03.safelinks.protection.outlook.com/?url=https%3A%2F%2Fyoutu.be%2FRVxKs3b-e4s%3Fsi%3Dg8-MURU7j02dtxap&data=05%7C02%7Cst10457924%40vcconnect.edu.za%7Cfa4267c8b3b946bcccc908dc557ba428%7Ce10c8f44f469448fbc0dd781288ff01b%7C0%7C0%7C638479236757280478%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=fMIskiL%2FMviDdOZYWcv%2B4v%2FekiHOZTD3U08P1qV0mJg%3D&reserved=0


5.Reference List:
⦁	https://www.bbc.com/news/world-africa-64660840
⦁	https://www.biography.com/musicians/michael-jackson
⦁	https://www.biography.com/musicians/michael-jackson
⦁	https://www.britannica.com/biography/Pele-Brazilian-athlete
⦁	https://www.britannica.com/biography/Diego-Maradona
⦁	https://www.britannica.com/biography/Elizabeth-II
⦁	https://www.britannica.com/biography/Tupac-Shakur
⦁	https://www.empireonline.com/people/paul-walker/
⦁	https://www.britannica.com/biography/Martin-Luther-King-Jr 
⦁	
Clayborne Carson
The Lott,R., Director, Martin Luther King, Jr., Research & Education Institute, and Martin Luther King Jr. Centennial Professor, Stanford University.
David L. Lewis
Lewis, D is the Julius Silver University Professor and a professor of history at New York University. He has authored and edited some ten books and has received two Pulitzer Prizes (for his volumes on W.E.B. DuBois), the Bancroft Prize, and the Francis Parkman Prize
⦁	https://www.nba.com/kobe-bryant-tribute
