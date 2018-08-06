---
layout: post
title: Make a Github Blog 깃허브 블로그 만들기 -1
tags:   [Git, Blog, Github, Github.io]
---

# Github 블로그 만들기 -1

Algorithm, Spring Framework 등 전공 관련 자료를 한 곳에 모아서 정리해야 할 필요성을 느끼던 도중, Github Blog에 대한 인지와 함께 매우 유용하다는 생각을 하게 되었다. Github Blog를 어떻게 시작하고 운영해야 하는 지에 대해 살펴보았으나 대부분의 사람들이 *Mac*이나 *Linux* 운영체제를 바탕으로 Github Blog를 만들고, 글을 올리는 방법에 대해 게시해 놓았기에 누구나 쉽게 **Windows** 운영체제에서 Github Blog를 만들고 글을 올리는 방법에 대한 포스팅을 해보려 한다.

### 1. Github Repository 생성

![new_repository](/images/Make_Github_Blog/Make_Github_Blog_1.png)
<br/>

자신의 Github 계정으로 로그인 한 뒤에 새로운 Repository를 생성한다.

### 2. Github 이름 정하기

![naming_github](/images/Make_Github_Blog/Make_Github_Blog_2.png)
<br/>

만들고자 하는 Github Blog의 이름을 정한다. *user_id.github.io* 각자 자신의 아이디 뒤에 .github.io를 붙여주길 바란다.
추가로 시작할 때 readme.md 파일을 자동으로 생성해 주는 것에 대해 체크를 하였다.

### 3. Setting 설정하기

![config_settings](/images/Make_Github_Blog/Make_Github_Blog_3.png)
<br/>

create repository를 누르게 되면 다음 화면이 나올 것이다. 위의 상단에 **Settings**를 눌러 이동해보자.

### 4. 주소 확인 및 branch 설정하기

![config_branch](/images/Make_Github_Blog/Make_Github_Blog_4.png)
<br/>

Settings에서 중간쯤 내려가다 보면 Github Pages라는 화면이 보일텐데 그곳에 자신의 블로그 주소를 볼 수 있을 것이다.
또한, **master branch**로 수정한 뒤에 save 버튼을 누르도록 하자.

### 5. 자신의 Github Blog 확인하기

![checking_github](/images/Make_Github_Blog/Make_Github_Blog_5.png)
<br/>

방금 확인 한 주소를 통해 자신의 블로그로 이동해보도록 하자. readme.md 파일에 적혀 있는 내용이 보여질 것이다.
이제 자신만의 Github Blog를 생성하였으니 수정하고, 글을 올려보도록 하자.

### 6. Github 수정 및 변경 파일 생성하기

![creat_new_file](/images/Make_Github_Blog/Make_Github_Blog_6.png)
<br/>

그림에서와 같이 **Create new file** 버튼을 눌러 새로운 파일을 생성해주자. 환경 설정 파일을 생성한다고 이해하면 좋을 것 같다.

### 7. _config.yml 파일 생성하기

![make_config.yml](/images/Make_Github_Blog/Make_Github_Blog_7.png)
<br/>

> Basic Option과 Build Setting 둘로 나눠서 접근을 해보면, Basic Option에는 Blog에 적을 자신의 정보를 나타낸다.
> Build Setting이 Github Blog를 설정하는 것을 나타내는 것인데, theme는 화면에 보여질 구조나 틀을 말하고 markdown은 posting을 어떠한 방식으로 할 것인지를 말하는 것이다.

![commit_config.yml](/images/Make_Github_Blog/Make_Github_Blog_8.png)
<br/>

이제 그럼 Commit new file 버튼을 눌러 _config.yml 파일을 commit 해보도록 하자.

![check_config.yml](/images/Make_Github_Blog/Make_Github_Blog_9.png)
<br/>

*_config.yml* 파일이 추가된 것을 확인해 볼 수 있을 것이다.

### 8. 글 올리기 및 수정하기

![checking_github](/images/Make_Github_Blog/Make_Github_Blog_10.png)
<br/>

변경한 theme가 잘 적용 되었는지 자신의 Github Blog 주소로 다시 들어가서 확인해보자. theme와 Basic Option에서 적은 내용이 잘 적용 된 것을 볼 수 있다. 하지만 아직 글을 작성하지 않았음에도, readme.md 파일에서 작성한 글이 반영되어 나타나는 걸 볼 수 있을 것인데 이에 대한 해결 방안은 여러가지가 있겠으나 간단하게 readme.md 파일에 적힌 내용을 지움으로써 해결하도록 하겠다.

![remove_readme.md](/images/Make_Github_Blog/Make_Github_Blog_11.png)
<br/>

readme.md 파일에 작성된 내용을 지웠다. 수정하는 방법은 가장 오른쪽 연필 모양의 아이콘을 눌러 작성된 내용을 지우면 된다.

![checking_github](/images/Make_Github_Blog/Make_Github_Blog_12.png)
<br/>

깔끔하게 지워진 모습의 화면을 확인할 수 있을 것이다. 이제 글을 작성하여 올려보도록 하자.

![add_post](/images/Make_Github_Blog/Make_Github_Blog_13.png)
<br/>

> Create new file을 눌어 반드시 **_posts** / **YYYY-MM-DD-Post.md** 형식으로 글을 작성하도록 한다.
> 또한, 아래 형식에 있어서 layout을 post로 작성해야 한다. title은 작성하는 글의 제목이라고 생각하면 좋다. 그 밑으로 자신이 작성하고 싶은 내용의 글을 작성하면 된다.

### 9. 게시된 글 확인하기

![add_post](/images/Make_Github_Blog/Make_Github_Blog_14.png)
<br/>

글을 작성하고 나서 commit을 하게 되면 자신이 작성한 글이 repository에 올라간 것을 확인 할 수 있을 것이다.

![checking_post](/images/Make_Github_Blog/Make_Github_Blog_15.png)
<br/>

이제 다시 자신의 Github Blog에 접속하여 글이 올라갔는지 확인해보도록 하자.

![checking_post](/images/Make_Github_Blog/Make_Github_Blog_16.png)
<br/>

글의 제목과 날짜를 확인해 볼 수 있으며 글의 제목을 누르게 되면, 작성한 글의 내용을 볼 수 있을 것이다.

계속해서 이런 방식으로 글을 작성한다면 매우 불편하다고 느낄 수 있을 것이다. 따라서 글을 작성하는 방법과 요령에 대해 다음 포스팅에서 설명하는 시간을 갖도록 하겠다.

## 참고 
<https://evanwill.github.io/go-go-ghpages/>