# Quiz Example

This project is a quiz application designed for the Android platform, developed using Kotlin. Users can answer a variety of questions to test their knowledge and track the number of correct answers.

## Key Features

### 1. Quiz Progression
- Users can answer a series of provided questions.
- Each question offers multiple choices, and users must select the correct answer.

### 2. Score Recording and Management
- Upon completing the quiz, the user’s score is calculated.

### 3. Simple and Intuitive User Interface
- A user-friendly, intuitive UI allows easy navigation.
- The results page displays the user’s score after the quiz.

## Project Structure

```
Quiz_Example/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/kr/co/ipdisk/quiz/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── QuestionActivity.kt
│   │   │   │   ├── ResultActivity.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_main.xml
│   │   │   │   │   ├── activity_question.xml
│   │   │   │   │   ├── activity_result.xml
│   │   │   │   ├── drawable/
│   │   │   │   ├── values/
│   │   │   │   ├── mipmap/
│   ├── build.gradle
│   ├── settings.gradle
│
├── gradle/
│   ├── wrapper/
│   │   ├── gradle-wrapper.jar
│   │   ├── gradle-wrapper.properties
├── build.gradle
├── gradlew
├── gradlew.bat
├── .gitignore
├── README.md
```

### Key Files and Directories

- **`app/src/main/java/kr/co/ipdisk/quiz/`**: Contains core application logic in Kotlin files.
  - **`MainActivity.kt`**: Entry point of the app, managing the quiz’s start screen.
  - **`QuestionActivity.kt`**: Displays each quiz question and handles user responses.
  - **`ResultActivity.kt`**: Displays quiz results after completion.

- **`app/src/main/res/`**: Contains application resources.
  - **`layout/`**: XML files defining the layout of each screen.
  - **`drawable/`**: Directory for image resources.
  - **`values/`**: Resource files defining colors, strings, themes, etc.

- **`gradle/`**: Contains files related to the Gradle build system.

## Installation and Run Instructions

### 1. Clone the Repository

Clone this project from GitHub to your local machine.

```bash
git clone https://github.com/yourusername/quiz-example.git
cd quiz-example
```

### 2. Open in Android Studio

Open the `quiz-example` directory in Android Studio.

### 3. Build and Run the Project

1. Build the project in Android Studio (`Build > Make Project`).
2. Run the app on a real device or emulator (`Run > Run 'app'`).
