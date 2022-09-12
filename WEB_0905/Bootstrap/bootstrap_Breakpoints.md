# 💡 Breakpoints



## Core concepts

* **Breakpoints are the building blocks of responsive design**.

  > 특정 뷰포트 또는 장치 크기에서 레이아웃을 조정할 수 있는 시기를 제어하는 데 사용

* **Use media queries to architect your CSS by breakpoint.** 

  > 미디어 쿼리는 브라우저 및 운영 체제 매개 변수 집합을 기반으로 스타일을 조건부로 적용할 수 있는 CSS의 기능 
  >
  > min-width : 미디어 쿼리에서 가장 일반적으로 사용 

* **Mobile first, responsive design is the goal.**

  > CSS는 최소한의 스타일을 적용하여 레이아웃이 가장 작은 중단점에서 작동하도록 한 다음 스타일에 레이어를 적용하여 더 큰 장치에 맞게 해당 디자인을 조정하는 것이 목표 => CSS 가 최적화되고 렌더링 시간이 향상되며 방문자에게 훌륭한 경험제공



## Available breakpoints 

> 그리드 계층이라고도 하는 6개의 기본 중단점이 포함 (소스 Sass 파일을 사용하는 경우 사용자 지정 가능)

| **Breakpoint** | **Class infix** | Dimensions |
| :------------: | :-------------: | :--------: |
|  Extra small   |     *None*      |   <576px   |
|     Small      |      `sm`       |   ≥576px   |
|     Medium     |      `md`       |   ≥768px   |
|     Large      |      `lg`       |   ≥992px   |
|  Extra large   |      `xl`       |  ≥1200px   |

> * 각 중단점은 너비가 12의 배수인 컨테이너를 편안하게 수용하도록 선택
>
> * 중단점은 또한 일반적인 장치 크기 및 뷰포트 치수의 하위 집합
>
> * 모든 사용 사례 또는 장치를 구체적으로 대상으로 하지는 않음 
>
>   (단, 이 범위는 거의 모든 장치에 구축할 수 있는 강력하고 일관된 기반을 제공)



## Media queries

>  모바일 우선으로 개발되었기 때문에 몇 가지 미디어 쿼리를 사용하여 레이아웃과 인터페이스에 적합한 중단점을 만든다. 
>
> 중단점은 대부분 최소 뷰포트 너비를 기반으로 하며 뷰포트가 변경됨에 따라 요소를 확장할 수 있다. 



