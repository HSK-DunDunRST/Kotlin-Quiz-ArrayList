## Android 퀴즈 애플리케이션

### 소개  
이 프로젝트는 **Kotlin**으로 개발된 **Android 퀴즈 애플리케이션**입니다.  
사용자는 주어진 문제를 풀고 점수를 기록할 수 있으며, 향후 **Room 데이터베이스** 및 **랭킹 시스템**을 추가하여 기능을 확장할 예정입니다.    

### 추후 개선점

- **Room 데이터베이스 적용**  
  - 기존 **ArrayList** 기반 문제 구조를 **Room DB**로 변경하여 데이터의 유동성이나 확장성을 개선할 예정입니다.  

- **랭킹 시스템 개선**  
  - 퀴즈 점수를 기록하고, 랭킹 기능을 추가할 예정입니다.  

---

## 필수 요구사항  
- Android Studio **Arctic Fox** 이상
- Java 17 이상
- Kotlin 1.5 이상  
- Gradle 7.x 이상  

## 프로젝트 구조  

```
Quiz_Example/
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

---

## 디렉토리 및 파일 설명  

### 1. `app/src/main/java/kr/co/ipdisk/quiz/`  
애플리케이션의 주요 **Kotlin 소스 코드**가 위치한 디렉터리입니다.  
- **`MainActivity.kt`**  
  - 앱의 시작 화면을 담당합니다.  
  - 사용자는 여기서 퀴즈를 시작할 수 있습니다.  

- **`QuestionActivity.kt`**  
  - 퀴즈 문제를 표시하고, 사용자의 답변을 처리합니다.  

- **`ResultActivity.kt`**  
  - 퀴즈 종료 후 결과 화면을 보여주며, 최종 점수를 출력합니다.

### 2. `app/src/main/res/`  
애플리케이션의 **리소스 파일**이 포함된 디렉터리입니다.  
- **`layout/`**  
  - UI 화면을 구성하는 XML 파일들이 포함되어 있습니다.  
  - `activity_main.xml`, `activity_question.xml`, `activity_result.xml` 파일이 각각 메인, 퀴즈, 결과 화면을 담당합니다.  

- **`drawable/`**  
  - 아이콘 및 배경 이미지와 같은 그래픽 리소스를 저장하는 폴더입니다.  

- **`values/`**  
  - 색상, 문자열, 테마 등의 설정이 포함된 XML 파일을 관리합니다.  

### 3. `gradle/`  
Gradle 빌드 시스템과 관련된 파일들이 포함된 디렉터리입니다.  
앱의 **의존성**을 관리하고 **빌드 설정**을 구성합니다.  

---
