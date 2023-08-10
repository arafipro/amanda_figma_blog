1. ヘッダーの画像を表示する範囲を指定

```css
.header {
  width: 100%;
  height: 856px;
}
```

2. 画像を配置、位置調整

```css
.header {
  width: 100%;
  height: 856px;
  /* 画像を配置 */
  background-image: url("/images/hero_image.jpeg");
  /* 画像の位置を調整 */
  background-position-x: center;
  background-position-y: 42%;
}
```

3. ヘッダーの要素を配置、クラスを設定

```html
<header class="header">
  <div class="header__menu">
    <div>
      <h1><a href="#">Amanda</a></h1>
      <p>a freelance blog writer</p>
    </div>
    <div>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
      <img src="images/vector.svg" alt="" />
    </div>
  </div>
  <div class="header__title">
    <div class="header__text">
      <h2>About self love & Relationships</h2>
      <p>
        Hi, I’m a Fitness enthusiast eager to share everything that i learned
        through my 5 year transformation
      </p>
    </div>
  </div>
</header>
```

4. 要素の配置を修正

```css
.header {
  width: 100%;
  height: 856px;
  background-image: url("/images/hero_image.jpeg");
  background-position-y: 42%;

  /* ここから最後まで追加 */
  .header___menu {
    justify-content: space-between;
    margin-right: auto;
    display: flex;
    padding-top: 57px;

    div {
      display: flex;
      align-items: center;
    }

    h1 {
      margin: 0 22px 0 80px;
    }

    ul {
      display: flex;
      width: 430px;
      height: 100%;
      justify-content: space-between;
      align-items: center;
    }

    img {
      margin: 0 54px;
      width: 25px;
      height: 14px;
      flex-shrink: 0;
    }
  }

  .header__title {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

    .header__text {
      text-align: center;
      width: 690px;
    }
  }
}
```

5. フォントの設定

```css
.header__menu {
  justify-content: space-between;
  margin-right: auto;
  display: flex;

  div {
    display: flex;
    align-items: center;
  }

  h1 {
    margin: 0 22px 0 80px;
    /* ここから追加 */
    color: #222;
    font-family: Inter;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: 100%; /* 24px */
  }

  p {
    color: #555;
    /* ここから追加 */
    font-family: Jaldi;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: 100%; /* 24px */
  }

  ul {
    display: flex;
    width: 430px;
    height: 100%;
    justify-content: space-between;
    align-items: center;

    /* liを追加 */
    li {
      font-family: Merriweather;
      font-size: 16px;
      font-style: normal;
      font-weight: 300;
      line-height: normal;
      letter-spacing: 0.48px;
      text-transform: uppercase;

      /* aを追加 */
      a {
        color: #222;
      }
    }
  }

  img {
    margin: 0 54px;
    width: 25px;
    height: 14px;
    flex-shrink: 0;
    /* ここから追加 */
    fill: #222;
  }
}

.header__title {
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;

  .header__text {
    text-align: center;

    /* h2を追加 */
    h2 {
      color: #222;
      text-align: center;
      font-family: Merriweather;
      font-size: 90px;
      font-style: normal;
      font-weight: 300;
      line-height: 120%; /* 108px */
      letter-spacing: -2.7px;
    }

    /* pを追加 */
    p {
      color: #444;
      text-align: center;
      font-family: Jaldi;
      font-size: 36px;
      font-style: normal;
      font-weight: 400;
      line-height: 48px; /* 133.333% */
    }
  }
}
```

6. 背景画像を白地で透過する

```css
.header {
  width: 100%;
  height: 856px;
  background-image: url("/images/hero_image.jpeg");
  background-position-y: 42%
	/* ここから追加 */
  background-color: rgba(255,255,255,0.5);
  background-blend-mode: lighten;
}
```

7. 位置の調整

```css
.header__text {
  text-align: center;
  /* ここに追加 */
  padding-bottom: 186px;
}
```
