<div align="center">

  # Hajo

  <img src="https://user-images.githubusercontent.com/84622281/231617435-1b4b61fe-0365-4968-962b-ec1427b2f089.jpg" width="200" height="200"/>

  <br/>

  **플랜을 관리하고 공유할 수 있는 앱**
  
</div>

<br/>

# 목차

[1. 개요](#개요)

[2. Project 진행](#Project-진행)

[3. 사용 기술 및 담당 역할](#사용-기술-및-담당-역할)

<br>

## 개요

- 대, 중, 소, 태스크로 나누어 플랜을 관리할 수 있다.
- 플랜을 공유하거나, 달성한 목표를 게시할 수 있다.
- 경쟁전으로 달성도를 비교해 의욕을 높일 수 있다.
- 다이어리로 달성 목표를 기록하고, 상점을 이용해 꾸밀 수 있다.

<br/>

## 구축 인원 및 기간

<b> - 기간 : 2022-07 ~ 2022-08 (총 7주) </b> <br/>
<b> - 인원 : 5명 (Android 3, Backend 2) </b>

<br>

## 프로젝트 기능 소개

<br>

### 로그인 / 홈화면

<img src="https://user-images.githubusercontent.com/84622281/231623729-0aed53aa-7fb3-4f75-9118-c7a8cb3b7e2d.png" width="1200" height="810"/>

<br>

### 플랜 관리 / 플랜 공유

<img src="https://user-images.githubusercontent.com/84622281/231623800-32c3bf62-d807-4967-806a-46d211136941.png" width="1200" height="810"/>

<br>

### 경쟁전 / 마이페이지 / 다이어리

<img src="https://user-images.githubusercontent.com/84622281/231623872-4cca21db-7029-4bf4-b7f6-f439800d7dc2.png" width="1200" height="810"/>

<br>

## Project 진행
- 기능 명세서, API 명세서 등 문서화를 하여 진행하였습니다.
- Jira Sprint와 GanttChart를 활용해 일정을 관리하였습니다.
- 모든 회의 내용을 회의록에 기록하고, 일정을 관리하고자 하였습니다.

<br>

## 사용 기술 및 담당 역할

### 사용 기술
<table>
<tr><th rowspan="1">Used</th><td>AndroidStudio / Kotlin / MVVM / Retrofit / Coroutine / Firebase</td></tr>
<tr><th rowspan="1">Used</th><td>Bottom Navigation / RecyclerView / ViewBinding / ViewModel / LiveData</td></tr>
<tr><th rowspan="1">New</th><td> Bottom Sheet / Calendar Custom Library </td></tr>
<tr><th rowspan="1">Collabo</th><td>Git / Jira / Notion / Mattermost / Swagger / GanttChart</td></tr>
</table>

<br/>

### 플랜 관리

<img src="https://user-images.githubusercontent.com/84622281/231627523-2529bef3-e37e-44bd-94d5-b4d5443afe73.jpg" width="1200" height="810"/>

<img src="https://user-images.githubusercontent.com/84622281/231627419-2f836ada-6085-45ed-b09c-10deda308dba.png" width="1200" height="810"/>

```
대, 중, 소, 태스크로 나누어 플랜을 등록하고 관리할 수 있도록 구현하였습니다. 상위 분류에 여러 플랜이 속할 수 있습니다.

월간보기 및 일별 보기 Calendar에 색, 아이콘으로 표시하고 확인할 수 있도록 하였습니다.

하루에 여러 개의 태스크를 등록할 수 있으며, 메모와 사진을 등록할 수 있습니다.
```

### 다이어리

<img src="https://user-images.githubusercontent.com/84622281/231629099-80387794-38f6-47a0-ab3e-aab60102f519.png" width="1200" height="810"/>


- 빈 화면으로 시작하여, 페이지 별로 이미지 또는 텍스트를 이동, 추가, 수정, 삭제할 수 있습니다. 

- 오브젝트는 Add 시 동적으로 화면에 생성되며, 내용 또는 위치를 수정하면 오브젝트 정보를 서버로 저장합니다.
ㄴ 이미지는 x, y, 이미지 정보 등이 저장됩니다.
ㄴ 텍스트는 글꼴, 색, 크기, 텍스트 내용 등이 저장됩니다.

- 페이지를 바꾸면 서버에서 가져온 해당 페이지의 정보를 바탕으로 오브젝트를 위치 시킨 곳에 설정하여 생성하여 보여줍니다.

- 상점에서 다이어리를 위한 스킨을 살 수 있습니다.
