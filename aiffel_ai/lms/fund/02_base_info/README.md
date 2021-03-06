# 목차
- 개발 환경 알아보기

# 개발 환경 알아보기
- 개론
- Ubuntu
- Python
- Tensorflow

- 클라우드 컨테이너 환경
    - 컨테이너란?
    > - 가상머신과 비슷함
    > - 더 효율적이고 가벼움
    > - 일종의 **일회용 가상 컴퓨터**
- 정확한 각각의 버전
    - Ubuntu 20.04.3
    - Python 3.9.7
    - TensorFlow 2.6.0

## Ubuntu
- 일종의 [운영 체제(OS)](https://jhnyang.tistory.com/16)
    - 복잡한 하드웨어를 쉽게 접근할 수 있도록 도와주는 프로그램
- [Ubuntu란?](https://dongdong-2.tistory.com/17)
    - Linux 기반의 OS
    - 공짜 OS
    - 20.04(2020년도 4월 출시)

## Python
- [다양한 프로그래밍 언어](https://www.youtube.com/watch?v=j5ogDOuqXqg)
    - 특별한 문제를 위한 언어 vs 범용성을 가진 언어
        - 적은 수요와 적은 공급으로 높은 월급을 받을 수 있음
- 버전 간 차이점 [3 vs 2](https://zetawiki.com/wiki/Python_%EB%B2%84%EC%A0%84_2%EC%99%80_3_%EC%B0%A8%EC%9D%B4)
    - print 방식
    - 형변환 방식

## Tensorflow
- 인공지능 특화 라이브러리!
    - 라이브러리란?
    > - 특정 기능을 위한 함수 클래스를 담고 있는 것
    > - 비슷한 개념으로 패키지, 모듈 등이 존재함
    > - [차이점](https://losskatsu.github.io/programming/function-module-package/#3-%ED%8C%A8%ED%82%A4%EC%A7%80%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC)
- 다른 인공지능 특화 라이브러리는?
    - PyTorch(파이토치)
    - Keras(케라스)

# 터미널(Terminal)
- CLI
- IDE
- 콘솔, 터미널, 쉘의 차이점

- 리눅스 기준 Ctrl + Alt + T를 통해 터미널을 열 수 있음
- **CLI(Command Line Interface)**
    - 명령어를 통해 컴퓨터를 사용함
    - 기본적인 [명령어](https://tutorial.djangogirls.org/ko/intro_to_command_line/)
    > ``` python
    > print("Hello World!")
    > ```
- **IDE(Integrated Development Environment)**
    - 터미널에서 코드를 한 줄씩 돌림
    - 불편한 경우가 있기 때문에 IDE를 통해 편하게 코드를 작성하고 저장함

- 터미널, 콘솔, 쉘의 [차이점](https://blog.naver.com/PostView.naver?blogId=asianchairshot&logNo=221383363419&redirect=Dlog&widgetTypeCall=true&directAccess=false)
    - 콘솔: 직접 명령어를 작성할 수 있는 입출력 장치(물리적)
    - 터미널: 로컬 또는 원격으로 컴퓨터와 접속할 수 있는 콘솔을 구현한 소프트웨어
    - 쉘: 실제로 명령어가 입출력이 되는 프로그램
    - 프롬프트: 사용자가 준비됨을 의미함

# 기본적인 명령어 모음
- whoami
- pwd
- ls -al
- cd dirs
- mkdir dirs
- rm -r dirs
- mv from to
- cp from to

### 문제!
- Home 디렉토리 밑에 dir1 라는 이름의 디렉토리를 생성하고, 그 밑에 dir2 를 또 생성하세요.
- dir2를 Home 디렉토리로 옮겨보세요.
- dir2를 다시 dir1 밑으로 복사해보세요.
- dir1 와 dir2를 모두 삭제하세요.

# 패키지 관리
- 설치된 패키지 확인하기
- 특정 패키지 존재 확인하기
- 최신 패키지로 업데이트 하기
- 특정 패키지 삭제

- 설치된 패키지 확인하기
    - sudo apt list --installed
- 특정 패키지 존재 확인하기
    - sudo apt list --installed | grep (패키지명)
- 최신 패키지로 업데이트 하기
    - sudo apt update -y && sudo apt upgrade -y
- 특정 패키지 삭제
    - sudo remove package

# 가상 환경
- 가상 환경이 왜 필요한가?
- 가상 환경 만들기
- 가상 환경 실행하기
- 가상 환경 종료하기

- 가상 환경이 왜 필요한가?
    - 버전이 상이한 2 프로젝트가 있다면, 각각의 라이브러리 버전관리가 필요함
- 가상 환경 만들기
    - python3 -m venv myvenv
- 가상 환경 실행하기
    - . myvenv/bin/activate
- 가상 환경 종료하기
    - deactivate