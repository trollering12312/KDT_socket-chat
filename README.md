# KDT_socket-chat

실습 원본 저장소 : https://github.com/ulgoon/sock-chat

## 실습 내용

commit 순서대로 진행됩니다

---

### express

1. app.js 파일 생성

2. 프로젝트 초기화 `npm init` 수행

3. express 설치 : `npm install --save express socket.io`

4. app.js 파일 작성

5. express 초기화 및 테스트 : `node app.js`실행후 `localhost:3000`접속해서 확인

6. route 디렉토리 생성후 index.js 파일 생성

7. indexRouter추가 : app.js, index.js 파일 각각 수정

8. clubsRouter 추가 : index.js 수정, clubs.js 생성

`http://localhost:3000/clubs/{팀명}` -> 팀명 출력

9. data.js 추가 : csv 파일 처리

`http://localhost:3000/clubs/{csv파일명}`
`http://localhost:3000/clubs/pl`

접속하면 json이 출력됨

10. ejs를 사용한 렌더링

ejs 설치 : `npm install --save ejs`

`index.ejs, app.js, index.js` 파일 수정

`http://localhost:3000`로 접속하면 렌더링 결과 확인 가능

ejs는 node.js의 템플릿 엔진으로 문법이 간단하고 서버의 데이터를 가져다 사용하거나 코드 실행이 가능하다

---

### socket

11. socket을 위한 렌더링

`app.js, chat.js, chatroom.ejs, chat.css` 수정

`http://localhost:3000/chat`으로 접속해 확인

12. 사용자 연결 처리

11번 URL접속시 `A user is now connected`로 연결 확인 가능

13. 연결 해제
