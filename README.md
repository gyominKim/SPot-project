🌱 SPot (Smart Pot)

📌 프로젝트 개요

SPot은 식물 관리에 어려움을 겪는 사용자를 위해 개발한 IoT 기반 스마트 화분 프로젝트입니다.
Android 앱을 통해 식물의 생육 정보를 조회하고, 예약 급수 및 수동 급수 기능으로 식물 관리를 지원합니다.
이 저장소는 Django 서버, 데이터베이스 연동 및 Python 기반 웹 크롤링 기능과 관련된 코드를 포함합니다.

✨ 주요 기능

1. 식물 정보 검색 및 자동 수집
데이터베이스에서 사용자가 검색한 식물의 정보 조회
식물 정보가 존재하지 않을 경우 웹 크롤링 실행
Selenium을 활용한 PictureThis 웹사이트 검색 자동화
BeautifulSoup을 활용한 식물 생육 정보 추출

2. 식물 정보 저장 및 제공
수집한 식물 정보를 Django 모델을 통해 데이터베이스에 저장
식물 이름, 학명, 수명, 햇빛 조건, 물 주기, 적정 온도 등 다양한 정보 관리
식물 이미지 다운로드 및 저장

🔄 식물 정보 검색 처리 과정
1. Android 앱에서 식물 이름 검색
2. Django 서버에서 데이터베이스 조회
3. 정보가 존재하면 기존 데이터 활용
4. 정보가 없으면 Selenium과 BeautifulSoup으로 웹 크롤링
5. 수집한 데이터를 MariaDB에 저장
6. 상세 정보 조회 API를 통해 Android 앱에 식물 정보 제공

👥 개발 참여 및 담당 역할

Python과 BeautifulSoup을 활용한 초기 크롤링 기능 구현
팀원과 협력하여 Selenium 기반 웹 크롤링 기능 개발
Android 앱과 Django 서버 간 통신 기능 개발 및 테스트 참여
기능 연동 과정에서 발생한 오류 점검 및 수정

🔗 관련 저장소
SPot Android App(https://github.com/gyominKim/SPot-project)
