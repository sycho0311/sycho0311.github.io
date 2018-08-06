---
layout: post
title: Make a Github Blog 깃허브 블로그 만들기 -1
tags:   [Git, Blog, Github, Github.io]
---

# Github 블로그 만들기 -2

Github 블로그 만들기 1편에 이어서 이번에는 나만의 github.io 블로그에 글을 효율적이며 쉽게 글을 작성하고, 관리하는 방법에 대해서 포스팅을 해보도록 하겠다.

### 1. 나만의 Github.io 블로그 Clone하기

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_17.png)
<br/>

자신의 Github Blog의 정보와 글을 담고 있는 github 주소로 이동하여 **Clone or download** 버튼을 클릭하여 Download ZIP을 선택하자. 이때 저장하는 위치는 자신의 컴퓨에서 쉽게 접근하고 편하게 찾을 수 있는 공간에 저장하도록 하자. 저장이 완료 되었다면 압축을 풀도록 하자.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_18.png)
<br/>

압축을 푼 상태에서 해당 폴더에 들어가 보면 자신이 작성한 파일들을 볼 수 있을 것이다. 여기서 이제 우리는 글을 작성하면 *_post* 폴더 안에 넣어주고, Github Blog의 정보와 글을 담고 있는 github 주소에 그 결과를 반영하면 되겠다. 자신의 컴퓨터에 Github Blog의 정보와 글을 담고 있는 것을 **local 저장소**라고 할 수 있고, 해당 github 주소를 **remote 저장소**라고 할 수 있다.

### 2. 글 작성 및 수정하기

**local 저장소**에서 글을 작성한 뒤 **remote 저장소**로 결과를 반영하는 것에 있어서는 3단계로 나눠서 구분할 수 있다.
``` 
git add 
git commit
git push
```
이렇게 3단계로 나눠서 작업을 진행해야 한다. 이러한 작업을 나는 *Visual Studio Code*를 사용하여 진행하였다.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_19.png)
<br/>

Visual Studio Code를 실행하면 가장 먼저 볼 수 있는 화면이다. 방금 github로부터 다운 받은 폴더의 위치를 찾아 열도록 하자.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_20.png)
<br/>

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_21.png)
<br/>

*_posts* 폴더 안에 지난 번에 작성한 글을 볼 수 있을 것이다. Visual Studio Code를 이용하여 글을 수정하는 것은 물론이고, 새로 글을 작성할 수도 있다. 물론 반드시 지난 번에 알려준 형식으로 글을 작성해야 한다. 이제 지난 번에 작성했던 글을 한번 수정해보도록 하겠다.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_22.png)
<br/>

7번째 라인에 글을 추가하였다. 이제 수정된 사항에 대해서 **remote 저장소**에도 반영을 하여 Github Blog에 변경 사항을 적용시켜 보도록 하자.