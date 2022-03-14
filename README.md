# tp_Calculator

기본적인 계산기를 구현

-연산자 우선순위에 의해 계산되는 계산기를 제작하는 것이 목표.

-html내부에 javascript구현이 아닌 js파일을 링크하여 구현할것,

-코드의 간략화

--1 commit--

 -onlclick을 이용해 table내부의 공간을 클릭하면 작동되도록 함.
 
 -다수의 배열을 사용해 (입력한 데이터를 저장 -> 숫자들의 병합 -> 곱셈,나눗셈 연산 우선실행 -> 덧셈,뺄셈 연산 실행)을 진행. (4개의 배열&for문 사용)
 
 -너무 많은 배열 및 for문 사용으로 인해 코드의 가독성이 매우 나쁨.

--2 commit--

-연산자의 첫순서입력, 중복입력 등에 대한 오류 수정.

-for에서 if를 사용해 연산자 발견시 실행하던 코드를 switch문으로 변경.

--3 commit--

-입력받은 데이터를 배열에 저장한후 10단위 이상의 숫자를 따로 병합하는 배열을 만드는 코드가 있었지만, 과정 단축화를 위해 입력받는 시점에서 temp에 수를 저장하고 연산자가 입력받을시
temp저장된 수와 연산자를 배열에 추가하고 temp를 초기화 하는 것으로 단축.

-위의 과정을 구현하기위해 연산자와 숫자의 입력을 받는 방식을 따로 구분함.(function getT => f NumPress , f getT)

-입력오류로 인한 결과 오류를 방지하기위해 alert를 사용하여 에러구분을 함.

-입력단계에서의 과정을 단축기킴으로 사용되는 배열 및 for문의 사용 빈도를 줄임.

-몇가지 변수 및 등등의 명(Name)을 가독성을 위해 변경함.
