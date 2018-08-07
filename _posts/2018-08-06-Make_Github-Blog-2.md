---
layout: post
title: Make a Github Blog 깃허브 블로그 만들기 -2
tags:   [Git, Blog, Github, Github.io]
---

# Github Blog 만들기 -2

Github 블로그 만들기 1편에 이어서 이번에는 나만의 Github Blog에 효율적이고 쉽게 글을 작성하고, 관리하는 방법에 대해서 포스팅을 해보도록 하겠다.

### 1. 나만의 Github Blog Clone하기

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_17.png)
<br/>

자신의 Github Blog의 정보와 글을 담고 있는 github 주소로 이동하여 **Clone or download** 버튼을 클릭 한 뒤, Download ZIP을 선택하자. 이때 저장하는 위치는 자신의 컴퓨에서 쉽게 접근하고 편하게 찾을 수 있는 공간에 저장하도록 하자. 저장이 완료 되었다면 압축을 풀도록 하자.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_27.png)
<br/>

> 물론 이 방법 이외에도 cmd 창이나 다음에 설명할 *Visual Studio Code* 편집기를 이용하여 Clone하는 방법 또한 존재한다. 명령어는 아래와 같다.
> clone 이후에 자신의 github URL을 copy하여 붙여넣길 바란다.

` git clone https://github.com/sycho0311/sycho0311.github.io.git `

clone 이전에 해야할 작업들(명령어)에 대해서 간단하게 집고 넘어가도록 하겠다.
```
git config --global user.name "user_name"
git config --global user.email "user_email@email.com"
git init
```

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_18.png)
<br/>

압축을 푼 상태에서 해당 폴더에 들어가 보면 자신이 작성한 파일의 목록을 볼 수 있을 것이다. 이곳에 있는 *_posts* 폴더 안에서 글을 작성 및 수정하고, Github Blog의 정보와 글을 담고 있는 github 주소에 그 결과를 반영하면 되겠다. 자신의 컴퓨터에 Github Blog의 정보와 글을 담고 있는 파일을 **local 저장소**라고 할 수 있고, 해당 github 주소를 **remote 저장소**라고 할 수 있다.

### 2. 글 작성 및 수정하기

**local 저장소**에서 글을 작성한 뒤 **remote 저장소**로 결과를 반영하는 것에 있어서는 3단계로 나눠서 구분할 수 있다.
``` 
1. git add 
2. git commit
3. git push
```
이렇게 3단계로 나눠서 작업을 진행해야 한다. 
글의 작성과 수정하는 작업을 진행하고, 진행한 작업의 내용을 github **remote 저장소**에 반영하기 위해서는 그에 맞는 적절한 편집기가 필요한데 이때 나는 *Visual Studio Code* 편집기를 사용하여 진행하였다.

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

7번째 라인에 글을 추가하였다.

### 3. Remote 원격 저장소에 Push, 변경사항 반영하기

이제 수정된 사항에 대해서 **remote 저장소**에도 반영을 하여 자신의 Github Blog에 변경 사항을 적용시켜 보도록 하자.
가장 먼저 **local 저장소**에 변경사항을 add 해야 한다.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_23.png)
<br/>

` git add --all `

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_24.png)
<br/>

` git commit -m "put your message" `

그 뒤 두번째로 commit을 해주도록 하고, 마지막으로는 **remote 저장소**에 push를 해야 한다.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_25.png)
<br/>

``` 
git remote add origin https://github.com/sycho0311/sycho0311.github.io.git
git remote -v
git push -u origin master
```
이곳에서 또한 origin 이후에 자신의 **remote 저장소** 주소를 copy하여 적어 넣어주길 바란다.

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_26.png)
<br/>

게시한 첫번째 글에 방금 작성한 글이 추가 되고 반영이 되는 것을 확인 할 수 있다. 이렇게 github 사이트에서 직접 글을 작성하게 되면 생기는 불편함을 **local 저장소**로 *Clone*하여 가져온 뒤에, 글을 작성하거나 수정하여 다시 **remote 저장소**에 반영한다면 지난번에 겪었던 어려움과 불편함을 굉장히 많이 해소 할 수 있을 거라 생각한다.

마지막으로 다음에는 markdown의 사용법을 통하여 글을 작성하는 요령에 대해 알아보도록 하겠다.

## 참고
<https://pages.github.com>
