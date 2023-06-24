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

+ 전처리
++ 주석 제거
++주석은 개발자가 자신과 개발자들의 코드 이해를 돕기위해 작성하는 메모입니다. 주석은 프로그램의 동작과 상관이 없으므로 전처리 단계에서 모두 제거됩니다.

++매크로 치환
++#define으로 정의한 매크로는 자주 쓰이는 코드나 상숫값을 단어로 정의한 것입니다. 전처리 과정에서 매크로의 이름은 값으로 치환됩니다.

++파일 병합
++일반적인 프로그램은 여러 개의 소스와 헤더 파일로 이루어져 있습니다. 컴파일러는 이를 따로 컴파일해 합치기도 하지만, 어떠한 경우는 전처리 단계에서 파일을 합치고 컴파일하기도 합니다.
