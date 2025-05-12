# smartphone-sensor_Machine-Learning-Deep-Learning

스마트폰 센서를 통해 정적과 동적인 활동을 분류하고 더 나아가 정적인 무슨 활동 or 동적인 어떤 활동을 예측하는 모델을 만드는 과정

단계 구분 예시
 단계1 : 정적(0), 동적(1) 행동 분류 모델 생성
 단계2 : 세부 동작에 대한 분류모델 생성
 단계1 모델에서 0으로 예측 -> 정적 행동 3가지 분류 모델링
 단계1 모델에서 1으로 예측 -> 동적 행동 3가지 분류 모델링

모델 통합
 두 단계 모델을 통합하고, 새로운 데이터에 대해서 최종 예측결과와 성능평가가 나오도록 함수로 만들기

성능 비교
 기본 모델링의 성능과 비교

성능 가이드
 Accuracy : 0.97 ~ 0.99
파이프라인 구성
 test 데이터를 입력하여, 전처리 및 예측결과가 나오도록 함수 구성

활동
    'STANDING': 0,
    'SITTING': 0,
    'LAYING': 0,
    'WALKING': 1,
    'WALKING_UPSTAIRS': 1,
    'WALKING_DOWNSTAIRS': 1
mapping을 통해 두 분류로 우선 분류시키고
정적에서 3가지 분류, 동적에서 3가지 분류를 진행하여 파이프라인으로 연결하는 과정

<img width="583" alt="image" src="https://github.com/user-attachments/assets/dfd751d8-48ab-4d34-b91a-172e35178962" />
