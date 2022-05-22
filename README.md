# OSS_Final_Proj_T2 - 북미
## ( Book美: The Beauty of Book )
--------------
## 목차
1. [프로젝트 설명](#1-프로젝트-설명)
2. [프로젝트 설치 방법](#2-프로젝트-설치-방법)
3. [프로젝트 사용 방법](#3-프로젝트-사용-방법)
4. [파일 목록](#4-파일-목록)
5. [개발자](#5-개발자)
6. [라이선스](#6-라이선스)
7. [연락처](#7-연락처)
--------------
## 1. 프로젝트 설명
Web app으로 HTML, Java Script, CSS, Bootstrap, jQuery, API, Ajax, git을 이용하여 제작했습니다. <br>
독서 기록장 사이트로, 도서 추천, 도서 검색, 독서 기록 서비스를 제공합니다.
______________
## 2. 프로젝트 설치 방법
### A. Local 환경에 설치하기
a. 터미널을 이용하여 로컬에 설치할 경로로 이동해줍니다.

```
$ cd 설치할 경로
```

b. 아래의 코드를 복사 후 붙여넣어, 코드를 모두 다운로드 해줍니다.

```
$ git clone git@github.com:swliris/OSS_Final_Proj_T2.git
```

c. 해당 설치 경로에 'OSS_Final_Proj_T2' 라는 이름의 폴더가 생겼다면, 설치에 성공한 것 입니다!
### B. Web 접속하기
[여기](https://swliris.github.io/OSS_Final_Proj_T2/)로 접속합니다.
______________
## 3. 프로젝트 사용 방법
A.	인터페이스(메인 화면)  
   a.	상단의 로고를 클릭하면 메인화면으로 이동할 수 있습니다.  
   b.	책이름으로 검색할 수 있는 도서 검색바가 있습니다. 검색 버튼을 누를 수 있습니다.  
   c.	배너 아래에는 도서 추천 목록이 보입니다.  
   d.	가장 아래에는 나의 독서기록장을 확인할 수 있습니다.  
  
B.	도서 추천  
   a.	국립중앙도서관에서 제공하는 추천도서 Open API를 사용하여 추천도서 목록을 메인 화면에서 가로 슬라이드 형식으로 유저에게 보여줍니다.  
   b.	추천도서는 문학, 인문과학, 사회과학, 자연과학 4가지 카테고리로 분류되어 있습니다.  
   c.	추천도서에 대한 간략한 정보(제목, 저자, 출판사, 출판연도)가 표지와 함께 사용자에게 보입니다.  
  
C.	독서 기록장  
   a.	“+ 독서기록장 추가” 버튼을 누르면 독서기록장 작성 페이지로 넘어갑니다.  
   b.	책 제목과 내용을 입력할 수 있는 칸이 있고, 내용 칸은 우측 하단을 드래그하여 크기를 조절할 수 있습니다.  
   c.	“저장” 버튼을 누르면 ‘독서 기록장을 저장하시겠습니까?’ 확인 문구가 팝업됩니다. “확인”을 누르면 다시 메인 화면으로 돌아와 ‘나의 독서기록장’에서 내가 쓴 내용을 리스트 형식으로 확인할 수 있습니다. “취소”를 누르면 독서기록장 작성 페이지에 그대로 있습니다.   
   d.	독서기록장은 가장 최근에 올린 순으로 정렬되어 있으며, 제목 옆의 휴지통 모양 “삭제” 버튼을 누르면 리스트에서 삭제됩니다.  
   e.	제목이나 내용이 없을 경우, 제목 또는 내용이 없다는 경고 팝업창이 뜨고 저장을 하지 않습니다.  
   f.	local storage를 사용하기 때문에 사용자 개인의 기록을 보관할 수 있습니다.  
  
D.	도서 검색  
   a.	상단의 검색 바에 책 이름을 쓰고 검색하면 도서 검색 결과 페이지로 이동합니다. 도서 검색 결과는 Kakao API 기반입니다. 검색 결과의 끝까지 스크롤을 제한 없이 내릴 수 있습니다.  
   b.	표지(썸네일), 책의 제목, 저자, 출판사, 출판연도, 간단한 요약을 확인할 수 있습니다. 출판연도와 요약 사이의 “독서기록장 쓰기” 버튼을 누르면 위에서 설명한 독서 기록장 기능을 사용할 수 있습니다.  
   c.	책 제목을 누르면 Kakao API가 제공하는 책의 자세한 소개를 보여주는 탭으로 이동합니다. 책소개와 리뷰, 판매정보를 확인할 수 있습니다. 이 탭에서 누르는 버튼들은 누르면 마찬가지로 Kakao에서 오픈소스로 제공하는 서비스를 그대로 이용할 수 있습니다.   
   d.	만약 검색결과가 없다면 “검색 결과가 없습니다.”라는 문구가 표시됩니다.   

_______________
## 4. 파일 목록
* OSS_Final_Proj_T2
    * index.html - 기본 페이지
    * report.html - 독서기록장 작성 페이지
    * search.html - 검색 결과 페이지
    * .gitignore - DS_store 무시
    * README.md - 프로젝트 관련 내용
    * LICENSE - MIT라이센스
    * css
        * style_report.css - report.html의 css파일
        * style_search.css - search.html의 css파일
        * style.css - index.html의 css파일
    * source
        * favicon.ico - 웹페이지 옆 작은 로고 사진
        * library.jpg - 검색창 뒤 배경사진
_______________
## 5. 개발자
<img width="20%" src="https://user-images.githubusercontent.com/100212793/169682252-33c86f98-8bbf-4c56-b172-52bea0bf2694.png"/>

### 임성우 (Leader)
* 개발자 소개
    * 성균관대학교 소프트웨어학과 2학년 재학 중
    * 2022 하계 산학협력 프로젝트 진행 중
* 프로젝트에서 맡은 부분
    * 프로젝트 총괄
    * Front-end (Design & html, css)
    * js
        * api 등을 통해 가져온 데이터 → 웹 페이지 적용
        * localStorage 관련
    * README 작성

<img width="20%" src="https://user-images.githubusercontent.com/100212793/169680886-47f8ac32-6052-4a06-a6a7-d13b5f47a464.PNG"/>

### 채시헌
* 개발자 소개
    * 성균관대학교 소프트웨어학과 2학년 재학 중
    * 소프트웨어학과 알리미 11기 회장
    * 산학협력 프로젝트 - Computer Vision을 이용한 사람의 포즈 인식 (LG U+)
* 프로젝트에서 맡은 부분
    * Back-end
    * js
        * popup 창 컨트롤
        * 국립 중앙 도서관 사서 추천 API, jQuery, Ajax를 이용한 사서 추천 도서 데이터 크롤링
    * README 작성

<img width="20%" src="https://user-images.githubusercontent.com/100212793/169684753-031adcb9-116a-4198-8724-c731ff7e52eb.PNG"/>

### 최중현
* 개발자 소개
    * 성균관대학교 소프트웨어학과 2학년 재학 중
    * 소프트웨어융합대학 5,6대 학생회
    * (전) 알고리즘 동아리 NPC, 정보보안 동아리 HIT
* 프로젝트에서 맡은 부분
    * Back-end
    * Kakao 도서검색 API, jQuery, Ajax를 이용하여 도서 검색, 스크롤 구현 js 작성
    * README 작성
_______________
## 6. 라이선스
이 프로젝트는 MIT 라이선스 조건에 따라 라이선스가 부여됩니다.
This project is licensed under the terms of the MIT license.
_______________
## 7. 연락처
임성우
* [github](https://github.com/swliris)
* e-mail : swliris@g.skku.edu

채시헌
* [github](https://github.com/SiHeonChae)
* e-mail : sean1106@g.skku.edu

최중현
* [github](https://github.com/Choi-Jung-Hyeon)
* e-mail : fourmi103@g.skku.edu
