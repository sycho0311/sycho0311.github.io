---
layout: post
title: Look into the OSI 7 Layer
tags:   [OSI, OSI 7 layer]
---

# OSI 7 Layer 살펴보기

이번 포스팅에서는 **OSI 7계층 모형(Open Systems Interconnection Reference Model)**에 대해서 알아보는 시간을 갖도록 하겠다. Web Application을 개발하는 데 있어서 OSI 7 Layer를 알고, 어떤 식으로 동작하는 지에 대해 이해하는 것이 필요하다는 생각에 이번 기회를 통해 정리해보도록 하겠다. 컴퓨터공학 전공자라면 한번쯤은 OSI 7계층 모형에 대해 들어보았지만 막상 설명하기는 어려운 개념이라고 할 수 있다. OSI 7계층에 대해 알고는 있지만 확실하게 개념이 확립되지 않은 분들이 이 글을 통해 각자 나름의 정리가 되었으면 한다.

### 1. OSI 7계층 모델

OSI 7계층 모델이란 국제 표준화 기구 ISO(International Standard Organization)에서 만든 원활한 통신을 위한 약속, 규약 혹은 절차를 의미한다. 데이터 교환 및 통신시에 기종마다 방식이 다르다면 혼선이 생기고 어려움이 있기 때문에 공통 표준의 필요성에 의해 생겨났다고 볼 수 있다. 데이터 교환 및 통신에 있어서 신뢰성이 있으며, 오류가 없고 복구가 가능하는 것을 포함한다. 각 계층구조마다 하는 역할이 있으며, 이러한 계층구조가 7계층으로 구성되어 있다.

![new_repository](/images/Look_Into_OSI_7_Layer/Look_Into_OSI_7_Layer_1.png)
<br/>

### 2. 통신 기초

각 계층마다 하는 역할과 기능에 대해서 알아보기 전에 통신 시스템의 흐름 및 통신이 어떤 식으로 동작하는 지에 대해 잠시 집고 넘어가도록 하자. 상위 계층과 하위 계층 간의 하는 역할에 대해 살펴보겠다.

![new_repository](/images/Look_Into_OSI_7_Layer/Look_Into_OSI_7_Layer_2.png)
<br/>

상위 계층에서 하위 계층에게 필요 서비스를 요청하면, 하위 계층에서는 상위 계층에게 해당 서비스를 제공하고 제공받은 서비스를 이용하여 통신에 사용한다.

또한 호스트 A와 호스트 B가 통신을 한다고 가정하였을 때, 자신의 n계층은 상대방의 n계층과 통신을 한다. 다시말해 자신의 n계층은 상대방의 n계층과 통신을 하고, n-1계층은 n-1계층에 해당하는 상대방의 계층과 대등하게 통신을 한다는 것을 뜻한다.

![new_repository](/images/Look_Into_OSI_7_Layer/Look_Into_OSI_7_Layer_3.png)
<br/>



