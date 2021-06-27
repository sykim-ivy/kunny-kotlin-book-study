# kunny-kotlin-book-study
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-sa/4.0/)


차세대 안드로이드 개발자를 위한: 커니의 코틀린 도서의 2부에서 다루는 **Simple Github** 예제 애플리케이션을 빈 플젝부터 (책시점보다) 최신 기술 및 버전 반영하여 재작성한 저장소입니다.

## 예제 목록

각 장에서 완성하게 되는 코드는 주제별로 구분되어 있는 브랜치로 확인할 수 있습니다.

각 브랜치는 직전의 브랜치를 기반으로 작성됩니다. (예: ``arch-components-lifecycle`` 브랜치에는 직전 브랜치인 ``rxjava-rxbinding``을 기반으로 구현되었으므로, ``RxJava`` 와 ``RxBinding``이 모두 적용되어 있는 상태입니다)

| 브랜치 | 언어 |  장 | 제목 | 책에서 다루는 내용 |
| --- | -- | --- | --- | --- |
| [java](https://github.com/kunny/kunny-kotlin-book/tree/java) | Java | 10 | Simple Github 예제 프로젝트 소개 | 자바로 작성한 Simple Github 예제 프로젝트 설명 |
| [kotlin-step-1](https://github.com/kunny/kunny-kotlin-book/tree/kotlin-step-1) | Java + Kotlin | 11 | 코틀린 변환 1단계: 컨버터로 자바 코드를 코틀린 코드로 변환하기 | Simple Github 예제 프로젝트에 코틀린 개발환경 설정, 컨버터를 사용하여 UI 코드를 코틀린으로 변환하는 절차 |
| [kotlin-step-2](https://github.com/kunny/kunny-kotlin-book/tree/kotlin-step-2) | Kotlin | 12 | 코틀린 변환 2단계: 코틀린다운 코드로 다듬기 | 11장에서 작업했던 코드에서 남은 자바 코드를 컨버터를 사용하여 코틀린으로 변환 후, 변환된 코드를 코틀린 답게 다듬는 방법 |
| [rxjava](https://github.com/kunny/kunny-kotlin-book/tree/rxjava) | Kotlin | 13 | 프로젝트 개선 1단계: RxJava 적용하기 | [RxJava](https://github.com/ReactiveX/RxJava)를 사용하여 이벤트를 기반으로 애플리케이션 동작을 처리하는 방법 |
| [rxjava-rxbinding](https://github.com/kunny/kunny-kotlin-book/tree/rxjava-rxbinding) | Kotlin | 13 | 프로젝트 개선 1단계: RxJava 적용하기 | [RxBinding](https://github.com/JakeWharton/RxBinding)으로 UI 이벤트를 RxJava로 처리하는 방법 |
| [arch-components-lifecycle](https://github.com/kunny/kunny-kotlin-book/tree/arch-components-lifecycle) | Kotlin | 14 | 프로젝트 개선 2단계: 안드로이드 아키텍처 컴포넌트 적용하기 | [Lifecycle](https://developer.android.com/topic/libraries/architecture/lifecycle.html)을 사용하여 액티비티 생명주기에 따른 동작 처리하기 |
| [arch-components-room](https://github.com/kunny/kunny-kotlin-book/tree/arch-components-room) | Kotlin | 14 | 프로젝트 개선 2단계: 안드로이드 아키텍처 컴포넌트 적용하기 | [Room](https://developer.android.com/topic/libraries/architecture/room.html)으로 손쉽게 SQLite 데이터베이스를 다루기 |
| [arch-components-viewmodel](https://github.com/kunny/kunny-kotlin-book/tree/arch-components-viewmodel) | Kotlin | 14 | 프로젝트 개선 2단계: 안드로이드 아키텍처 컴포넌트 적용하기 | [ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel.html)을 사용하여 액티비티 상태 보존하기 |
| [dagger-step-1](https://github.com/kunny/kunny-kotlin-book/tree/dagger-step-1) | Kotlin | 15 | 프로젝트 개선 3단계: 대거 라이브러리로 필요한 객체 제공하기 | [Dagger](https://google.github.io/dagger/)로 API 및 데이터베이스 접근에 필요한 객체를 필요한 곳에 제공하는 방법 |
| [dagger-step-2](https://github.com/kunny/kunny-kotlin-book/tree/dagger-step-2) | Kotlin | 15 | 프로젝트 개선 3단계: 대거 라이브러리로 필요한 객체 제공하기 | [Dagger](https://google.github.io/dagger/)로 각 액티비티의 ``ViewModel`` 및 리사이클러뷰 어댑터 객체 제공하기 |

## 빌드 환경

예제 애플리케이션 빌드에 사용하는 환경은 다음과 같습니다.

| 항목 | 버전 |
| --- | --- |
| Android Gradle Plugin | `3.0.1` |
| Build Tools | `27.0.2` |
| Minimum SDK | `15` |
| Compile SDK | `27` |
| Target SDK | `27` |

## 사용하는 라이브러리 및 버전

예제 애플리케이션에서 사용하는 라이브러리 및 버전은 다음과 같습니다.

| 이름 | 라이선스 | 버전 |
| --- | --- | --- |
| [Anko](https://github.com/Kotlin/anko) | [Apache License 2.0](https://github.com/Kotlin/anko/blob/master/LICENSE) | `0.10.3` |
| [Android Architecture Components](https://developer.android.com/topic/libraries/architecture/index.html) | Apache License 2.0 | `1.0.0` |
| [Android Support Library](https://developer.android.com/topic/libraries/support-library/index.html) | Apache License 2.0  | `27.0.2` |
| [Dagger](https://google.github.io/dagger/) | [Apache License 2.0](https://github.com/google/dagger/blob/master/LICENSE.txt) | `2.12` |
| [Glide](https://github.com/bumptech/glide) | [LICENSE](https://github.com/bumptech/glide/blob/master/LICENSE) | `4.1.1` |
| [Gson](https://github.com/google/gson) | [Apache License 2.0](https://github.com/google/gson/blob/master/LICENSE) | `2.7` |
| [Kotlin](https://github.com/JetBrains/kotlin) | [LICENSE](https://github.com/JetBrains/kotlin/tree/master/license) | `1.2.0` |
| [OkHttp](http://square.github.io/okhttp/) | [Apache License 2.0](https://github.com/square/okhttp/blob/master/LICENSE.txt) | `3.8.1` |
| [Retrofit](http://square.github.io/retrofit/) | [Apache License 2.0](https://github.com/square/retrofit/blob/master/LICENSE.txt) | `2.3.0` |
| [RxAndroid](https://github.com/ReactiveX/RxAndroid) | [Apache License 2.0](https://github.com/ReactiveX/RxAndroid/blob/2.x/LICENSE) |  `2.0.1` |
| [RxBinding](https://github.com/JakeWharton/RxBinding) | [Apache License 2.0](https://github.com/JakeWharton/RxBinding/blob/master/LICENSE.txt) | `2.0.0` |
| [RxJava](https://github.com/ReactiveX/RxJava) | [Apache License 2.0](https://github.com/ReactiveX/RxJava/blob/2.x/LICENSE) | `2.1.3` |








## 출처 저서 : '차세대 안드로이드 개발자를 위한: 커니의 코틀린' 

[교보문고](https://goo.gl/AczLBC) | [YES24](https://goo.gl/ZN82zG) | [알라딘](https://goo.gl/TybL2u) | [인터파크](https://goo.gl/YHGFbt)

- 참고한 원본 저서 예제 변경 내역은 [kunny-kotlin-book](https://github.com/sykim-ivy/kunny-kotlin-book/tree/master/CHANGELOG.md) 문서를 참조하세요.

- 원본 변경 내역은 [CHANGELOG](https://github.com/kunny/kunny-kotlin-book/tree/master/CHANGELOG.md) 문서를 참조하세요.
