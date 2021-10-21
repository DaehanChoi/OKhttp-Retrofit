# OKhttp-Retrofit


## 안드로이드에서 OkHttp를 사용하지 않을 경우
>1. HttpUrlConnection 연결
>2. Buffer 입출력 
>3. 각종 예외처리
> 등을 모두 직접해줘야하고 이것은 너무나 번거로운 일임

# Retrofit 이란?
> type-safe한 Http통신 client 라이브러리 -> '프로그램 동작이 잘 정의된'
> OkHttp위에서 돌아가게 됨 -> 내부에서 OkHttp Client를 디폴트로 선언한다.

## Gson으로 데이터 모델을 편리하게 json형태로 
```kotlin
1. Android에 Internet permission
<uses-permission android:name="android.permission.INTERNET" />

2. Gradle에 Gson 의존성 추가
implementation 'com.google.code.gson:gson:2.8.8'

3. Gson 객체 생성 및 메소드 이용 
val gson = Gson()
val json = gson.toJson(Models)
        
```
