![스크린샷 2023-06-16 오전 12 11 10](https://github.com/ljunseok0514/home-work/assets/73566234/88be82a0-08ba-4525-b914-645aa83f91e8)
<br>1. 스프라이트 기법으로 스타일링
```css
.site_li {
  position: relative;
  margin-bottom: 8px;
  background: url(./../mission-01/images/rank.png) no-repeat;
}

.W3C {
  background-position: 157px 4px;
}
.Web_Standards {
  background-position: 157px -41px;
}
.CSS_ZenGarden {
  background-position: 157px -17px;
}
.MDN {
  background-position: 157px 4px;
}
```
<br>2. ol 요소에서 제공하는 기본숫자를 보이지 않게 한 후 counter-reset, counter-increment속성을 활용해 스타일링했다<br>
```css
ol {
  list-style: none;
  padding-left: 0;
  counter-reset: index;
}

.site_name::before {
  position: absolute;
  counter-increment: index;
  content: "" counter(index);
  display: inline-block;
  height: 16px;
  width: 16px;
  text-align: center;
  font-size: 11px;
  line-height: 16px;
  border-radius: 4px;
  background: #a3a3a3;
  color: #fff;
  margin-right: 4px;
  left: -0px;
}
```
