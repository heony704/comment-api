## 댓글 CRUD를 위한 json-server api

댓글 CRUD를 위해 `json-server` 라이브러리를 이용해서 `Vercel`에 구축된 서버입니다.

[https://comment-api.vercel.app/comments](https://comment-api.vercel.app/comments)에 `GET` 요청시 `data.json` 파일에 기록된 데이터를 확인할 수 있습니다.

API 사용법에 대한 추가정보는 [`json-server` 공식문서](https://www.npmjs.com/package/json-server)를 참고하세요.

| method | url |
| ------ | --------------------- |
| GET | /comments |
| GET | /comments/{commentId} |
| POST | /comments |
| PUT | /comments/{commentId} |
| DELETE | /comments/{commentId} |
      
API 호출 예시:
- 한페이지에 4개의 게시물이 보이고, 최근 게시물부터 정렬해서 3페이지를 보고 싶은 경우
- GET `/comments?_page=3&_limit=4&_order=desc&_sort=id`

## Reference

- https://github.com/kitloong/json-server-vercel
