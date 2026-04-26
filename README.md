# CS360-Mobile-Architect-Programming
## Overview
This project is a fully functional Android mobile application designed to help users track their weight, set fitness goals, and monitor progress over time. The application focuses on simplicity, usability, and reliability, providing a streamlined experience without unnecessary complexity.

The app demonstrates core mobile development concepts including user authentication, persistent data storage, multi-activity navigation, and platform-specific features such as SMS notifications.

## Features
- User account creation and login
- Goal weight setting and tracking
- Daily weight entry logging
- Dashboard displaying progress
- SMS notifications when goals are reached
- Local data persistence using SQLite

## Tech Stack
- **Language:** Java  
- **IDE:** Android Studio  
- **Platform:** Android (API 26+)  
- **Database:** SQLite  
- **Architecture:** Multi-Activity Android App  
- **Other Features:** SMS Notification Integration  

## Application Architecture

The application is structured using a multi-activity design:

- **LoginActivity**
  - Handles user authentication and account creation

- **GoalActivity**
  - Allows users to define and update weight goals
  - Enables SMS notification settings

- **Dashboard (Main Activity)**
  - Displays user progress
  - Allows entry of new weight data
  - Serves as the central navigation hub

### Data Flow
- User inputs are validated and stored locally using SQLite
- Data persists across sessions
- Activities communicate using intents and shared data updates

## Reflection

### Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The goal of this project was to design and develop a fully functional mobile application that allows users to track their weight over time, set personal fitness goals, and monitor progress in a structured way. The application needed to support persistent data storage, user authentication, and a clear interface for entering and reviewing weight data.

This app was designed to address the need for a simple and reliable way to track personal health metrics without unnecessary complexity. Many existing solutions are overloaded with features, so this project focused on delivering a streamlined experience where users can quickly log data, view progress, and stay accountable to their goals.

### What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
The application includes several core screens:
- Login and account creation screen
- Goal-setting screen
- Dashboard for tracking and displaying weight entries
- SMS notification integration for goal completion

Each screen was designed with simplicity and clarity in mind. Navigation between screens is straightforward, and the layout prioritizes readability and ease of interaction. The dashboard serves as the central hub, allowing users to quickly view their progress and input new data without unnecessary steps. The UI design was successful because it minimized friction for the user. Instead of overwhelming the user with options, the interface focuses only on essential features. This aligns with user-centered design principles by reducing cognitive load and making the app intuitive to use from the first interaction.

### How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
The development process followed a structured, incremental approach. The app was built in stages, starting with core functionality such as user authentication and navigation, then expanding into data storage, UI refinement, and additional features like SMS notifications.

Key techniques included:
- Breaking the application into separate activities (Login, Goal, Dashboard)
- Implementing modular logic for handling user input and data storage
- Using SQLite for persistent local storage
- Iterative testing after each major feature was added

This approach can be applied in future projects by reinforcing the importance of building a stable foundation before adding complexity. Incremental development reduces debugging complexity and allows for more controlled progress.

### How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
Testing was performed continuously throughout development using the Android emulator. Each feature was tested individually after implementation, including login functionality, data entry, goal tracking, and navigation between screens.

Breakpoints and debugging tools were used to trace issues, particularly when handling activity transitions and data persistence. Testing revealed several issues early on, such as application crashes during login and inconsistencies in data handling, which were resolved through step-by-step debugging.

This process is important because it ensures that each component works correctly before integrating it into the larger system. It also helps identify edge cases and prevents small issues from becoming larger problems later in development.

### Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
One area that required problem-solving was integrating features across multiple activities while maintaining consistent data flow. Ensuring that user data, such as weight entries and goals, updated correctly across different screens required careful handling of intents and stored data.

Another challenge was implementing SMS notifications in a way that aligned with Android permission requirements. This required understanding how permissions are requested and handled at runtime, as well as ensuring that the feature worked without introducing unnecessary complexity.

These challenges required adapting the initial design and refining the implementation to ensure both functionality and usability were maintained.

### In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
The strongest component of this project is the overall integration of the application’s core features into a cohesive system. The combination of user authentication, persistent data storage using SQLite, and a functional dashboard proved my understanding of mobile application architecture. The implementation of SMS notifications shows an ability to work with platform-specific features and permissions, which is an important aspect of Android development. Together, these components reflect both technical capability and an understanding of user-focused design.
