<img width="425" alt="스크린샷 2023-06-14 오전 12 40 35" src="https://github.com/ljunseok0514/home-work/assets/73566234/f301d6f3-b382-48fa-82c9-fc571f5a20cf">
<br>
1.이미지는 figure태그로 감싸서 img태그로 넣었고, figcation으로 캡션을 달앗다.<br>
2.grid를 이용하여 레이아웃을 구현했다

```css
.container{
grid-template: repeat(3, 1fr) / 112px repeat(3, 1fr);
}

.content_top {
  grid-area: 1/1/1/-1;
}

.content_top {
  grid-area: 1/1/1/-1;
}

.news_img_box {
  grid-area: 2/1/4/1;
}
```
<br>
3.border에 gradient를 줬다.

```css
border-image: linear-gradient(to right, #a9a9a9 0%, #ffffff 100%);
  border-image-slice: 1;
```
