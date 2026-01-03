# FE
android frontend

## 사용 기술 스택 
Kotlin, Android Studio(ver. Narwhal 3 Feature Drop | 2025.1.3)

## 라이브러리
기능관련 : 캘린더뷰, 날씨, Glide, kizitonwose, 카카오 로그인 <br />
데이터베이스 관련 : Room, Retrofit

---  

### 📝 Commit Convention

커밋 메시지는 아래의 형식을 준수하여 작성합니다.

#### Format
`[type]: 요약 제목 (task 유형)`  
&nbsp;&nbsp;&nbsp;&nbsp;`"본문: 필요한 경우에 선택적으로 작성"`

#### Example
`[feat]: 로그인 UI 구현 (로그인)`  
&nbsp;&nbsp;&nbsp;&nbsp;`코드에 대하여 상세 기술`

    
#### 💡 Type & Task 상세

#### Type
✨ **[feat]**: 새로운 기능 추가  
🐛 **[fix]**: 버그 수정  
📝 **[docs]**: 문서 수정 (README, 주석 등)  
🎨 **[style]**: 코드 스타일 변경 (포맷, 세미콜론 등)  
♻️ **[refactor]**: 리팩토링 (기능 변화 없음)  
✅ **[test]**: 테스트 코드 추가 / 수정  
🧽 **[chore]**: 빌드 설정, 패키지 관리 등 기타 작업  
⚡ **[perf]**: 성능 개선  
👷🏻 **[ci]**: CI/CD 설정 변경  
🌱 **[build]**: 빌드 관련 파일 수정 (예: Gradle)  
⏪ **[revert]**: 이전 커밋 되돌리기  
🖼 **[design]**: 기능 변경 없이 UI만 변경 (CSS 등)  
🔄 **[rename]**: 파일 혹은 폴더명을 수정만 한 경우  
🗑 **[remove]**: 파일을 삭제만 한 경우  

#### Task
**로그인**: 로그인 구현 관련  
**옷 사진 등록 & 자동 분류**: 옷 사진 업로드 및 자동 분류  
**디지털 옷장**: 옷장 조회 및 필터  
**코디 일기**: 옷 착용 이력 저장 및 일기 구현  
**일정 / 날씨 연동**: 날씨 표시  
**착용 이력**: 통계 요약 및 집계  
**데모데이 패키징**: 데모 시연용 패키징

---

### 💻 Code Convention

#### 1. 이름 규칙
🏷 **기본**: camelCase  
🏷 **상수**: UPPER_CASE  
🏷 **boolean**: is + camelCase (ex. isHuman = True)  

➕ **연산자**: 앞뒤 공백 사용

#### 2. 함수 및 주석 규칙
중괄호 사용을 준수하며, 함수 작성 시 **KDoc** 주석을 사용합니다.

```kotlin
/**
* 함수 기능 설명
*
* @param[name]
* @param[name]
* @return
*/
```

🔗 KDoc 참고: [기본 사용법](https://dev-jewon.tistory.com/21) / [블록 태그](https://velog.io/@dudgns0507/Kotlin-KDoc으로-코틀린-코드-문서화하기-feat.-Dokka)

  
#### 3. 📂 폴더 구조  
Task별로 폴더를 구성하며 내부 구조는 아래 형식을 따릅니다.

📁 Task (Task명)  
    ├── ui: Activity, Fragment, Adapter

    ├── data: Entity, Dao, Database

    └── network: NetworkUtil

Example:  
📁 Task (로그인)     ├── ui / data / network  
📁 Task (옷 사진 등록 & 자동 분류)     ├── ui / data / network
