# 📕 프로젝트명

### ✔️ 챗봇 기반의 스마트 도서관 통합 서비스
![image](https://user-images.githubusercontent.com/115389344/230848713-d9cc4670-07dd-482d-a0dc-8dabdcf80c1e.png)

# 📃 프로젝트 소개 

### ✔️ 챗봇 기반의 스마트 도서관 통합 서비스 프로젝트입니다.

스마트 도서관은 시민들을 위해 역, 주민센터 주변에 배치된 책 자판기 형태의 작은 도서관입니다. 현재 사용자들이 스마트 도서관에 어떤 책이 어디 있는지 혹은 운영시간에 대한 정보를 얻기 위해서는 각 스마트 도서관별 홈페이지에 접속하여 찾아야 하는 불편한 구조를 가지고있습니다. 이러한 점을 개선하고자 여러 스마트 도서관들을 통합하여 도서 위치, 대출 현황, 이용시간 등을 하나의 서비스에서 제공할 수 있는 통합 챗봇 서비스를 개발하게 되었습니다.

이러한 서비스를 통해 사용자들은 원하는 도서를 도서명, 작가명, 위치명들을 기반으로 검색하고 원하는 장르의 도서들을 추천받을 수 있으며 이용시간, 연체, 반납 등 도서관별 문의 사항에 대한 정보를 하나의 통합된 서비스를 통해 얻을 수 있습니다.

# 🛠 기술 스택

### ▪ 언어
<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/java-FC4C02?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/jquery-0769AD?style=for-the-badge&logo=jquery&logoColor=white">

### ▪ 주요 라이브러리
<img src="https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"> <img src="https://img.shields.io/badge/konlpy-ECD53F?style=for-the-badge&logo=konlpy&logoColor=white"> <img src="https://img.shields.io/badge/sentence transformers-EB1923?style=for-the-badge&logo=sentencetransformers&logoColor=white"> <img src="https://img.shields.io/badge/scikit learn-F7931E?style=for-the-badge&logo=scikit learn&logoColor=white">  <img src="https://img.shields.io/badge/pymysql-4479A1?style=for-the-badge&logo=pymysql&logoColor=white">

### ▪ 프레임워크
<img src="https://img.shields.io/badge/spring boot-6DB33F?style=for-the-badge&logo=spring boot&logoColor=white"> <img src="https://img.shields.io/badge/flask-000000?style=for-the-badge&logo=flask&logoColor=white"> <img src="https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white"> 

### ▪ 데이터베이스
<img src="https://img.shields.io/badge/mariadb-003545?style=for-the-badge&logo=mariadb&logoColor=white">

### ▪ 서버
<img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=for-the-badge&logo=Apache Tomcat&logoColor=white"> <img src="https://img.shields.io/badge/Amazon EC2-FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white"> <img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white">

### ▪ 개발 툴
<img src="https://img.shields.io/badge/Google Colab-F9AB00?style=for-the-badge&logo=Google Colab&logoColor=white"> <img src="https://img.shields.io/badge/Eclipse IDE-2C2255?style=for-the-badge&logo=Ecilpse IDE&logoColor=white"> <img src="https://img.shields.io/badge/VS code-2F80ED?style=for-the-badge&logo=VS code&logoColor=white"> <img src="https://img.shields.io/badge/HeidiSQL-76B900?style=for-the-badge&logo=HeidiSQL&logoColor=white">

### ▪ 협업 툴
<img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=Github&logoColor=white"> <img src="https://img.shields.io/badge/Noiton-A5915F?style=for-the-badge&logo=Noiton&logoColor=white"> <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white">

# 🖥 시스템 구조

![image](https://user-images.githubusercontent.com/115389344/233107279-6ab12ac7-42cd-4c2e-8f7e-504d179a7b61.png)

1) 웹 서버(Spring)에서 채팅을 통한 사용자 요청(string형 발화문)
2) 요청된 string 객체 데이터 서버(Flask)로 전달
3) 검색, 추천, 문의, 예외 등 총 4개의 클래스로 분류 (Intent Classification)
4) 검색, 추천 의도 시 데이터베이스에 접근하여 데이터 SELECT
5) 의도별 답변 정보 취합 후 json 객체에 저장하여 웹 서버로 반환
6) 답변 메세지 출력 (검색된 도서 대출 가능 시 대여 버튼, 불가능 시 반납 알림 버튼 활성화)
7) 사용자의 요청 시 마다 초기화, 반복

# 💡 주요 기능

- 전체 도서 목록 , 이용 안내 방법 확인

- 도서 검색 (위치명, 작가명, 도서명)

- 도서 추천 (장르명)

- 문의 사항 (운영시간, 연체, 1인 대출 권수 등)

# 🔍 참고 자료

- 시연 동영상 : https://youtu.be/hZ_O2oySuOs
- 참고 링크(블로그) : https://velog.io/@min0731/%EC%B1%97%EB%B4%87-%EA%B8%B0%EB%B0%98-%EC%8A%A4%EB%A7%88%ED%8A%B8-%EB%8F%84%EC%84%9C%EA%B4%80-%ED%86%B5%ED%95%A9-%EC%84%9C%EB%B9%84%EC%8A%A4-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B81 
