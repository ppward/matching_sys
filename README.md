# ❤️ 원트 (OneT)

</br>

## 📌 프로젝트 소개 — 원트 (OneT)
**원트(Onet)** 는 SNS 데이터를 기반으로 개인의 성향과 가치관을 분석해, 내면적인 궁합을 중심으로 이성 매칭을 제안하는 데이트 매칭 플랫폼입니다. 사용자의 다섯 가지 핵심 가치관과 무의식적 호감 편향을 수치화하여, 보다 정서적·지향점이 유사한 상대를 추천합니다.

</br>

## 🎯 프로젝트 목적

기존의 데이트 매칭 플랫폼은 외모 중심의 피상적인 기준에 치우쳐 있어, 진정한 성향 일치나 가치관 기반의 매칭이 어려운 구조였습니다. OneT는 SNS 해시태그 및 사용자 활동 데이터를 분석하여 개인의 관심사와 성격을 예측하고, 사전에 구성된 질문지를 통해 가치관을 정밀하게 측정합니다.
이를 통해 사용자는 시각적 첫인상에 의존하지 않고, 자신과 높은 성향 유사도를 가진 이성과 더욱 직관적으로 연결될 수 있습니다.

</br>

## 🔑 주요 기능

### Instagram 기반 SNS 성향 데이터 수집
- 라즈베리파이를 활용해 Instagram OAuth 인증 과정을 redirect 방식으로 구현하여 사용자의 SNS 활동 데이터에 접근
- 사용자 게시물 및 해시태그 데이터를 분석해 주요 관심사와 성향을 추출
### 가치관 기반 질문지 시스템 구축
- 사전 설계된 10개의 심층 질문지를 통해 사용자 가치관(예: 관계 중심성, 여가활동 성향 등)을 수치화
- 각 사용자 응답을 수치로 변환해 매칭 알고리즘 입력값으로 활용
### Flask 기반 평균 거리 유사도 매칭 API 구현
- 수치화된 성향 데이터를 기반으로 사용자 간 평균 거리(Euclidean Distance)를 계산
- Flask API 서버를 통해 실시간 매칭 결과를 프론트엔드에 제공
### RDB와 S3 연동 기반 데이터 관리 시스템
- AWS S3에 배포된 환경에서 MySQL 기반 RDB를 구성해 사용자 정보 및 성향 데이터를 구조화
- 사용자 질문 응답, SNS 분석 결과, 매칭 기록 등 관계형 테이블로 관리
### Faiss 기반 벡터 검색 + LangChain 적용 대화형 에이전트
- Globe API를 통해 사용자 성향 데이터를 벡터로 변환 후 Faiss를 활용한 유사도 검색 적용
- LangChain을 활용해 사용자 응답 흐름을 분석하고, 맞춤형 대화 시나리오를 구성하는 대화형 AI 에이전트 구현
### React Native 기반 모바일 클라이언트 구현
- 사용자 인증, 질문 응답, 추천 결과 확인, 대화형 에이전트 사용 등의 주요 기능을 모바일 앱으로 구현
- 직관적인 UI/UX 설계를 통해 사용자가 성향 기반 매칭 결과를 손쉽게 확인 가능

</br>

## 📦 기술 스택

### ⚡️Language & Framework  
![javascript](https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000000)
![python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![reactnative](https://img.shields.io/badge/reactnative-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

### 🌐 Server
![nginx](https://img.shields.io/badge/nginx-009639?logo=nginx&logoColor=fff&style=for-the-badge)
![flask](https://img.shields.io/badge/flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![express](https://img.shields.io/badge/express-black?logo=express&logoColor=fff&style=for-the-badge)

### 🗄️ Database
![AWS S3](https://img.shields.io/badge/AWS_S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge)
![mysql](https://img.shields.io/badge/mysql-4479A1?logo=mysql&logoColor=fff&style=for-the-badge)

### 🛠 Tools
![jira](https://img.shields.io/badge/jira-0052cc?style=for-the-badge&logo=jira&logoColor=white)
![confluence](https://img.shields.io/badge/confluence-172B4D?style=for-the-badge&logo=confluence&logoColor=white)
![git](https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white)
![github](https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white)  

### 🧰 etc
![raspberrypi](https://img.shields.io/badge/raspberrypi-A22846?logo=raspberrypi&logoColor=fff&style=for-the-badge)
![ubuntu](https://img.shields.io/badge/ubuntu-E95420?logo=ubuntu&logoColor=fff&style=for-the-badge)

</br>

## 👋️ 팀원 소개  
| 이름 | 역할 |  
| ---- | ---- |  
| [이슬희](https://github.com/leeseulhui) | AI, Backend |
| [박기표](https://github.com/ppward) | Frontend(React Native), Server |  
| [강구용](https://github.com/kangguyong) | Backend |
