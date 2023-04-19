# 프로젝트명 : 챗봇 기반의 스마트 도서관 통합 서비스

![image](https://user-images.githubusercontent.com/115389344/230848713-d9cc4670-07dd-482d-a0dc-8dabdcf80c1e.png)

# 프로젝트 소개 

챗봇 기반의 스마트 도서관 통합 서비스 프로젝트입니다.

스마트 도서관은 시민들을 위해 역, 주민센터 주변에 배치된 책 자판기 형태의 작은 도서관입니다. 현재 사용자들이 스마트 도서관에 어떤 책이 어디 있는지 혹은 운영시간에 대한 정보를 얻기 위해서는 각 스마트 도서관별 홈페이지에 접속하여 찾아야 하는 불편한 구조를 가지고있습니다. 이러한 점을 개선하고자 여러 스마트 도서관들을 통합하여 도서 위치, 대출 현황, 이용시간 등을 하나의 서비스에서 제공할 수 있는 통합 챗봇 서비스를 개발하게 되었습니다.

이러한 서비스를 통해 사용자들은 원하는 도서를 도서명, 작가명, 위치명들을 기반으로 검색하고 원하는 장르의 도서들을 추천받을 수 있으며 이용시간, 연체, 반납 등 도서관별 문의 사항에 대한 정보를 하나의 통합된 서비스를 통해 얻을 수 있습니다.

# 기술 스택

- 언어 : Python(3.9.16), Java(openJDK 17), JavaScript, HTML, CSS
- 주요 라이브러리 : tensorflow(2.11.0), konlpy(0.6.0), sentence-transformers(2.2.2), sklearn, pymysql(1.0.3)
- 프레임워크 : Spring Boot(3.0.5), Flask(2.2.2), Fastapi(0.95.1)
- 데이터베이스 : MariaDB(5.2.14)
- 서버 : Apache Tomcat 9.0 , AWS (EC2, RDS)
- 개발 툴 : Colab, Eclipse, VScode,	HeidSQL
- 협업 툴 : Github, Slack, Notion

# 시스템 구조

![image](https://user-images.githubusercontent.com/115389344/233107279-6ab12ac7-42cd-4c2e-8f7e-504d179a7b61.png) 

# 주요 기능

- 전체 도서 목록 , 이용 안내 방법 확인

- 도서 검색 (위치명, 작가명, 도서명)

- 도서 추천 (장르명)

- 문의 사항 (운영시간, 연체, 1인 대출 권수 등)

# 참고 자료

- 시연 동영상 : https://youtu.be/Q35C48ziSsQ
