# Reverse-Engineering-Chapter-1

### 용어 정의

[**기계어(Machine Language)**](): 0 1로 이루어진 기계언어

[**어셈블리어(Assembly Language)**](): 기계어를 사람이 이해하기 쉽게 표현한 언어

[**어셈블러(Assembler)**](): 어셈블리어를 기계어로 번역해주는 놈

[**저급 언어(Low-Level Language)**](): 어셈블리어보다 사람이 이해하기 쉽게 만든 언어 (ex. C, C++, Go, Rust)

[**고급 언어(High-Level Language)**](): 저급 언어를 대규모 프로그램 개발에 적합하게 설계된 언어

[**컴파일러(Compiler)**](): 저급, 고급 언어를 기계어로 번역해주는 놈

[**바이너리(Binary)**](): 일반적인 경우 프로그램을 의미. 그 외, 이진 데이터

[**인터프리팅(Interpreting)**](): 컴파일 없이 그때그때 코드를 기계어로 번역하는 것 (Phton, JS가 이런 방)

+ 컴파일(Compile)의 정확한 의미는 어떤 언어로 작성된 소스 코드(Source Code)를 다른 언어의 목적 코드(Object Code)로 번역하는 것입니다. 이런 맥락에서, 소스 코드를 어셈블리어로, 또는 소스 코드를 기계어로 번역하는 것 모두 컴파일이라고 볼 수 있습니다.

### 본론

C언어로 작성된 코드는 일반적으로 전처리(Preprocess), 컴파일(Compile), 어셈블(Assemble), 링크(Link)의 과정을 거쳐 바이너리로 번역
