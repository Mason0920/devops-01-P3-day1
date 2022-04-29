# project3-microservices-day1

Serverless를 이용하여 마이크로서비스의 작은 예시를 실습
https://github.com/cs-devops-bootcamp/project3-microservices-day1

- Step-1 : Serverless 기반 legacy 시스템 배포 및 테스트 학습 
- Step-2 : SQS 이용하여 Producer-Consumer 구조 개발 학습
- Step-3 : SNS-SQS 환경에서, SNS 발행서버 구현
- Step-4 : “부산도너츠" 마이크로서비스 시나리오 환경구성

# DAY1 알고 넘어가기
---
- 환경변수 : .env file vs env commmand?
- 버전관리 : asdf를 사용하여 항상 버전에 민감하자. global, local로 각 컴퓨터별 디렉토리별로 버전을 적용할 수 있다. 그래서 .tool-versions이 있는 것이다.
- package.json을 잘 읽어보고 무엇을 뜻하는지 알자
- serverless.yml
- cURL, man curl 명령어에 대한 설명이 나온다.
- init.sql : 왜 복잡한 UID를 사용할까? 외부 노출에 민감한 경우 간단한 인덱스는 사용하지 않는다.
- 스키마 : 
    - Pub/Sub pattern : 하나의 토픽, 시나리오를 사용한다. 메시지를 보내는데, 등록된 사람 모두에게 보내자.
    - Producer/Consumer pattern : 