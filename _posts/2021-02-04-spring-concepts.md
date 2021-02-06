---
date: 2021-02-04 16:27:21
layout: post
title: "스프링은 도대체 뭘까 [上]"
subtitle: 스프링을 시작하며 어려웠던 점들
description: 스프링 / 스프링 MVC / 스프링 부트 뭐가 뭔지 헷갈리게 하던 것들을 정리해봤다. 
image: https://user-images.githubusercontent.com/77602977/107124108-26a3ca80-68e5-11eb-8e4b-d404523763de.png
optimized_image: https://user-images.githubusercontent.com/77602977/107124108-26a3ca80-68e5-11eb-8e4b-d404523763de.png
category: dev
tags:
- java
- spring
author: NHNkimjaemin
paginate: true
---
> _사진: 스프링 홈페이지_

## 스프링, 도대체 뭘까
스프링을 처음 다뤄보면서 느꼈던 어려웠던 개념들과 헷갈리는 용어들에 대해 내 나름의 방식으로 정리해보았다. 알아두면 다른 자료를 찾아볼 때에도 도움이 될 것이다.


### 스프링? 스프링 MVC? 스프링 부트?
결론부터 말하자면, 스프링은 자바 어플리케이션 개발을 위한 프레임워크이고, 스프링 MVC는 스프링 프레임워크 내의 웹 프레임워크이다. 스프링 부트는 스프링을 좀 더 빠르고 간편하게 사용할 수 있게 해주는 프레임워크이다.

#### Spring Framework
> "Spring handles the infrastructure so you can focus on your application."

스프링은 자바 기반의 어플리케이션 개발에 사용되는 프레임워크이다. 개발자가 어플리케이션 레벨의 개발에만 집중할 수 있도록 만들어졌다.

스프링은 여러 계층으로 이뤄진 모듈의 집합이다. 코어계층, 웹계층, 데이터 계층 등으로 이루어져있다. 하단 그림에서 보듯이 각 계층별로 모듈들이 속해있고, 모듈구조이기 때문에 원하는 개발에 따라 필요한 모듈만 선택해서 개발할 수 있다.
![spring-layers](https://docs.spring.io/spring-framework/docs/3.0.x/spring-framework-reference/html/images/spring-overview.png)

#### Spring MVC
그 중, 스프링 MVC 프레임워크는 웹개발에 사용되는 MVC 패턴을 쉽게 사용할 수 있게 스프링에서 제공하는 프레임워크이다.<br><br>
여기서 MVC란, Model-View-Controller 패턴을 말한다.<br>
**Model**은 데이터를 담당하는 부분을 말한다.<br>
**View**는 데이터를 사용자가 원하는 형태로 보여주는 부분을 말한다.<br>
**Controller**는 사용자 요청을 받고, 해당하는 모델을 가져와 뷰로 넘겨주는 부분을 말한다.<br>


#### Spring Boot
스프링 부트는 스프링을 더 쉽게 사용할 수 있도록 기본적으로 사용하는 설정과 보일러플레이트 코드 정도를 제공하는 프레임워크이다. <br><br>
 스프링도 경량 프레임워크라고 하지만, 설정에 시간이 많이 소요된다고한다. 그런 설정이 필요한 경우에는 어쩔 수 없지만 많은 프로젝트에서는 유사한 설정을 사용하는데, 그때마다 일일이 똑같은 설정을 반복해야했다. 스프링 부트에서는 그런 부분을 확 줄이고자 기본적인 설정을 선택하기만 하면 바로 실행할 수 있는 상태로 프로젝트를 제공해준다. 스프링 기반이기 때문에 원한다면 세부설정을 변경할 수도 있다. <br>

[<u>Spring initializr</u>](https://start.spring.io/)를 통해 쉽게 스프링 부트 프로젝트를 생성해볼 수있다.


### 다음 포스트 예고
다음 포스트는 **Spring Bean**과 **Spring IoC Container**에 대해 작성 중이다. 
원래는 한 포스트에 다 하려했는데, 분량이 많아져서 두 포스트로 쪼개게 되었다.
쓰면서 공부하게 되다보니까 생각보다 오래걸려서 차근차근 해봐야겠다.

> 내용오류 지적/ 오타 알림/ 질문 모두 환영입니다. 필요하시면 아래 댓글!


<p style="color:#999999; font-size: 18px;line-height: 1.5;font-style: italic">
출처:<br>
1) https://spring.io/projects/spring-framework <br>
2) https://docs.spring.io/spring-framework/docs/3.0.x/spring-framework-reference/html/overview.html <br>
3) https://dzone.com/articles/spring-boot-vs-spring-mvc-vs-spring-how-do-they-compare<br>
4) https://dailyheumsi.tistory.com/159<br>
5) https://study-develop.tistory.com/9<br>
</p>
