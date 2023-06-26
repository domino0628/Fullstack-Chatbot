# Package.json
<br/><br/>
※JSON : "키-값" 쌍으로 이루어진 데이터 객체를 사용하여 데이터를 구조화하는 등의 약속이 있는 텍스트 형식이다.
<br/><br/>
ex)
```
{
  "name": "John",
  "age": 30,
  "isStudent": false
}

```

-언제 생길까?
 1. 프로젝트 생성 : 프로젝트 디렉토리를 생성하고, 디렉토리에서 npm 명령어를 통해 새로운 프로젝트를 초기화할때 생성
 
 ※ npm install : 패키지 의존성을 설치하는 방법이다

<br/><br/>
 2. 의존성 설치: 이미 존재하는 프로젝트에 새로운 패키지를 추가하거나 의존성을 설치할 때 npm install 등의 
 명령어로 패키지 정보와 버전 정보가 package.json에 자동으로 저장됨
 
 
 ※ Package-lock.json
 
 패키지 버전 충돌이나 의존성 업데이트로 인한 호환을 방지하려고, 의존성 버전을 고정시켜 프로젝트를
 일관된 상태로 유지시키는 역할
 
 <br/>
 ※ 의존성 : 프로젝트에서 사용되는 외부 패키지,라이브러리,모듈
 
 <br/><br/>
 ex) package.json 파일에서 의존성 정의
<br/><br/>
 {
  "dependencies": {
    "express": "^4.17.1"
  }
}
<br/><br/>
  express는 패키지 이름, 4.17.1은 버전을 나타냄
<br/><br/>
  ex) ^4.17.1 : 부버전 업데이트를 허용함 ex 4.18.1은 허용, 5.1(주버전)은 불허
 
 <br/><br/><br/>
 
-scripts : 프로젝트의 스크립트 명령어를 정의함

 ex) ```"scripts": {
  "build": "webpack --mode production",
  "start": "nodemon index.js"
}```
<br/><br/><br/><br/>
 nodemon index.js :  nodemon은 서버 파일인 index.js를 감시하고 변경이 감지되면 자동으로 서버를 재시작
 <br/><br/><br/>
 자동 재시작 이유? 실시간 업데이트: 서버를 재시작함으로써, 변경 내용을 실시간으로 반영할 수 있기 때문에
 <br/><br/><br/>
 실행방법 : npm run <script-name>, 따라서 npm run start 하면 실행된다.
 <br/><br/><br/>
 왜 쓸까? : 명령 프롬프트에 직접 nodemon index.js를 입력하긴 번거롭기 때문
 


