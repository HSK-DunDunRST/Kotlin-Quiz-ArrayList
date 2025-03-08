# 퀴즈 예제

이 프로젝트는 Android 플랫폼을 위한 퀴즈 애플리케이션으로, Kotlin을 사용하여 개발되었습니다.  
아직 완성된 프로젝트가 아니며, 현재 상태로 코드 실행하면 문제가 발생할 수 있습니다.  

## 예정중인 개발
- Room 데이터베이스 적용
- Room 데이터베이스 적용 완료 시 문제 ArrayList 구조에서 변경.
- 랭킹 시스템 개선



## 주요 기능

### 1. 퀴즈 진행
- 사용자는 제공된 일련의 질문에 답할 수 있습니다.
- 각 질문은 여러 선택지를 제공하며, 사용자는 정답을 선택해야 합니다.

### 2. 점수 기록 및 관리
- 퀴즈가 완료되면 사용자의 점수가 계산됩니다.

### 3. 간단하고 직관적인 사용자 인터페이스
- 사용하기 쉽고 직관적인 UI가 있어 편리하게 탐색할 수 있습니다.
- 결과 페이지에서 퀴즈 완료 후 사용자의 점수를 확인할 수 있습니다.

## 프로젝트 구조

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

### 주요 파일 및 디렉터리

- **`app/src/main/java/kr/co/ipdisk/quiz/`**: Kotlin 파일로 된 애플리케이션의 핵심 로직이 들어 있습니다.
  - **`MainActivity.kt`**: 앱의 시작 화면을 관리하는 진입점입니다.
  - **`QuestionActivity.kt`**: 각 퀴즈 질문을 표시하고 사용자의 응답을 처리합니다.
  - **`ResultActivity.kt`**: 퀴즈 완료 후 결과를 표시합니다.

- **`app/src/main/res/`**: 애플리케이션의 리소스가 들어 있는 폴더입니다.
  - **`layout/`**: 각 화면의 레이아웃을 정의하는 XML 파일들입니다.
  - **`drawable/`**: 이미지 리소스를 위한 디렉터리입니다.
  - **`values/`**: 색상, 문자열, 테마 등을 정의하는 리소스 파일들입니다.

- **`gradle/`**: Gradle 빌드 시스템과 관련된 파일들이 들어 있습니다.
