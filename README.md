# HBNU 2023 Summer CE Hackathon
## 목적
2023년도 하계 컴퓨터공학과 해커톤은 지역사회의 문제를 해결하기 위하여 단순히 수준 높은 기술의 연구 개발을 목표로 하는 것이 아니라 현존하는 기술을 활용하여 해결책(Solution)을 도출하여 혁신을 도출하는 것을 목표로 한다. 

## 배경
지역 대학은 매년 대학 구성원의 한 해 연구 성과를 정리하여 관리하는 작업을 수행하는데 논문 사사가 있는 논문을 제출해야 할 때와 논문 사사가 없는 논문을 제출해야 하는 상황이 있다. 따라서 매년 행정직원은 대학구성원이 제출한 논문성과를 개별적으로 확인하여 논문사사의 표기 유무를 확인해야 하고 이로 인하여 2~3주 불필요한 초과근무를 수행해야 하는 문제가 있다. 또한, 사람이 논문을 제출하고, 제출된 논문을 평가하는 과정을 거치다보니 발생할 수 있는 인적오류(Human Error)로 인하여 매년 구성원의 불만사항이 높아지고 있다. 

## 문제정의
지역 대학의 사사표기 유무를 검증하는 작업을 대신하는 프로그램을 작성하라. 

## 입력
- pdf 파일의 한국어, 영어논문

## 출력
- 사사표기 유무(있음, 없음, 판단불가)
- output.csv 형태로 결과를 출력함
- 논문의 저자를 구분하여 각각 표기해야 함
- 출력 파일의 형태는 다음과 같음
|저자|소속대학|논문제목|사사표기여부|

## 출력 예제
- 저자: 최창범1, 장수영1, Jane Doe2
- 소속: 1한밭대학교 2한국대학교
- 제목: 세상을 변화시키는 방법
- 사사표기: This work was supported by Institute of Information & communication Technology Planning & Evaluation (IITP) grant funded by the Korea government (MSIT) (No.2022-0-00194, Analysis and Research of 5G Standard Patents)

## openai사용시 config.py 작성
    OPENAI_KEY = "Chat Bot KEY"
    INPUT_PATH = "./input"
    OUTPUT_PATH = "./output"

## 평가유의사항
- 테스트 데이터에 대해서 정확한 결과를 반환하는 경우 유로 API를 사용하는 경우 호출API 횟수를 적게 가져가는 팀이 가산점을 받는다.
- 유료 API 호출 횟수도 같은 경우 실행시간이 짧은 팀이 우승한다. 
  


