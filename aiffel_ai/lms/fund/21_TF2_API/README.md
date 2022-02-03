# 목차

# TF2
- 간단한 이미지 분류를 통해 알아보자
- 적합한 모델링 방식을 택하면 편해짐
- 크게 3 종류로 나눌 수 있음
    - Sequential
    - Functional
    - Model Subclassing
## Sequential
- 순차적
- 입력 1가지 출력 1가지
- 예제 [링크](https://www.tensorflow.org/tutorials/quickstart/beginner)
## Functional
- 함수로 묶어준 형태
- 입력과 출력을 다양하게 변경할 수 있음
- 예제 [링크](https://www.tensorflow.org/guide/keras/functional)
## Subclassing
- 근본적으로 함수형과 다른 것은 없음
- __init__ 이라는 메서드에 레이어 구성
- call() 이라는 메서드 안에서 forward
- 깊게 다루면 의도하지 않은 에러 발생 위험이 있음
- 예제 [링크](https://www.tensorflow.org/tutorials/quickstart/advanced)
# gradientTape
- model.compile에 있는 각 요소를 풀어서 사용할 때 사용
    - optimizer
    - loss
    - metrics
