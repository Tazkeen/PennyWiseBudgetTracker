# PennyWiseBudgetTracker

Penny Wise - Budget Tracker App
Penny Wise is an Android budget tracking application designed to help users manage their monthly spending, organise expenses into categories, set budget goals, view spending analytics, and stay motivated through achievements.
The app was created as a personal finance tool for users who want a simple and clear way to understand where their money is going. It focuses on everyday budgeting needs such as recording expenses, tracking categories, monitoring monthly budget limits, and reviewing spending behaviour.

App Screens
Logo:
 
 
Login Page
The login screen controls access to the app and ensures that only the correct user can enter the budget tracker.
 
 
Registration Page
The registration screen represents the process of creating a user account. In this demo version, the app uses fixed login credentials, but the registration page is included to show the full user journey.
 

 
Home Page
The home screen acts as the control centre of the app. It gives the user a quick overview of their finances and provides access to all main features.
The home page displays:
•	Total amount spent
•	Monthly budget goal
•	Remaining budget
•	Highest spending category
•	Navigation to expenses, categories, budget, analytics, and achievements
 



 
 
Expenses Page
The expenses page allows users to record and view their spending. Users can enter an expense name, choose a category, add an amount, and record the date of the expense.
This screen helps users keep track of day-to-day spending and understand how small expenses affect their monthly budget.
 


 
Categories Page
The categories page allows users to organise expenses into meaningful groups. Categories make it easier to understand spending patterns.
Example categories include:
•	Food & Dining
•	Transportation
•	Health Care
•	Shopping
•	Entertainment
•	Bill & Utilities
 

 
 
Budget Page
The budget page allows users to set a monthly budget goal. It also shows the current spending total and the remaining budget amount.
This screen helps users plan their spending and stay within their financial limits.
 

 

 

 
Analytics Page
The analytics page helps users understand their spending behaviour. It displays spending totals by category and shows how much of the monthly budget has been used.
This allows users to identify areas where they may be overspending.
 

 

 
 
Achievements Page
The achievements page motivates users by rewarding good financial habits. Achievements are unlocked based on actions such as recording expenses, staying within budget, and organising categories.
 

 
 
Custom Features Documentation
Feature 1: Budget Management
Users can create a monthly budget and track their spending. The app compares expenses against the budget and displays the remaining balance. This helps users manage their finances and avoid overspending.
Key Functions
•	Set a monthly budget
•	Track expenses
•	View remaining budget
•	Monitor spending progress

Feature 2: Smart Notification System
The app includes a notification system to keep users informed about their spending habits.
Key Functions
•	Alerts users when they are close to their budget limit.
•	Sends notifications when a budget has been exceeded.
•	Provides daily reminders to log expenses.
•	Displays clear and actionable messages.
•	Allows users to enable or disable notifications in Settings.

 
Purpose of the App
The purpose of Penny Wise is to provide a simple and practical way for users to manage their personal finances. Many people struggle to keep track of their spending, especially when purchases are made across different categories.
Penny Wise solves this by giving users one place to:
•	Record expenses
•	Group expenses by category
•	Set a monthly budget
•	View spending progress
•	Analyse spending habits
•	Stay motivated with achievements
The app encourages better financial awareness and helps users make smarter money decisions.

Design Considerations
Simplicity
The app was designed to be easy to use. Each screen has a clear purpose, and the navigation is straightforward. Users can move from the home screen to any major feature without confusion.
User-Friendly Layout
The interface uses clean layouts, readable text, and simple buttons. The goal was to make the app understandable even for users who are not highly technical.
Budget-Focused Structure
Each feature supports the main purpose of the app: helping users manage money. The expenses, categories, budget, analytics, and achievements screens all work together to give users a complete view of their spending.

Consistent Navigation
The home page acts as the main dashboard. From there, users can access each feature. Each feature screen also includes a back button so users can easily return to the dashboard.
Motivational Features
The achievements screen was included to encourage users to build better financial habits. This makes the app feel more engaging and rewarding.
Offline Demo Functionality
The app currently stores information during the app session. This makes it simple to test and demonstrate without requiring a database or internet connection.
Technologies Used
•	Android Studio
•	Java
•	XML layouts
•	Gradle
•	GitHub
•	GitHub Actions

Project Structure
The project is organised using a standard Android Studio structure.
PennyWise3/
|-- app/
|   |-- src/
|   |   |-- main/
|   |   |   |-- java/com/example/pennywise/
|   |   |   |-- res/layout/
|   |   |   `-- AndroidManifest.xml
|-- build.gradle.kts
|-- settings.gradle.kts
 
Main Java files include:
•	Login.java
•	Register.java
•	Home.java
•	ExpensesActivity.java
•	CategoriesActivity.java
•	BudgetActivity.java
•	AnalyticsActivity.java
•	AchievementsActivity.java
•	BudgetStore.java

GitHub Usage
GitHub was used to manage the source code for the project. It provides version control, which makes it easier to track changes, organise development, and keep a backup of the app.
Using GitHub helped with:
•	Tracking project changes
•	Keeping the app files organised
•	Maintaining a history of updates
•	Preparing the project for submission
•	Making the project easy to share and review

Recommended GitHub workflow:
git add .
git commit -m "Create Penny Wise budget tracker app"
git push origin main
Each commit should describe the work completed, such as adding login functionality, creating the budget screen, or updating the README documentation.
GitHub Actions
GitHub Actions can be used to automatically build and check the Android project whenever changes are pushed to GitHub.
This helps ensure that the project still compiles successfully after updates.
Example GitHub Actions workflow:

name: Android Build

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Set up JDK
        uses: actions/setup-java@v4
        with:
          distribution: temurin
          java-version: 17

      - name: Grant execute permission for Gradle
        run: chmod +x gradlew

      - name: Build debug APK
        run: ./gradlew assembleDebug

The workflow performs the following steps:
1.	Downloads the project from GitHub.
2.	Sets up Java for the Android build.
3.	Gives Gradle permission to run.
4.	Builds the debug version of the app.
This is useful because it checks the project automatically and helps catch build errors early.

How to Run the App
1.	Open the project in Android Studio.
2.	Allow Gradle to sync.
3.	Select an emulator or connected Android device.
4.	Click the Run button.
5.	Login using:
Username: @edinShand
Password: ediShand
 
Future Improvements
Possible improvements for future versions include:
•	Saving expenses permanently using a local database
•	Adding Firebase authentication
•	Adding charts for spending analytics
•	Allowing users to edit and delete expenses
•	Adding monthly reports
•	Supporting multiple users
•	Exporting budget summaries
Conclusion
Penny Wise is a simple and practical Android budget tracker designed to help users understand and control their spending. The app includes the core features expected from a budgeting tool: login, registration, expense tracking, categories, budget goals, analytics, and achievements.
GitHub was used to manage the project, and GitHub Actions can be used to automatically build and verify the app. This makes the development process more reliable and professional.

