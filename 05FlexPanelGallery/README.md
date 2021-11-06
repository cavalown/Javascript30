# Flex Panel Gallery

## HTML

---

## CSS

### :first-child

[參考 MDN](https://developer.mozilla.org/zh-TW/docs/Web/CSS/:first-child)
`偽元素`，將上一層視為父類別時，該父類別的長子元素。

### :last-child

同上的概念，即為最後一個元素。

### :nth-child

同上的概念，指定第幾個元素，從 0 開始。

---

## JS

- ### EventTarget.addEventListener()

  [參考 MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/EventTarget/addEventListener)
  透過註冊監聽器到 EventTarget 上，根據觸發的條件，啟用指定的 callback function。

  - 監聽事件： - click: 滑鼠點擊。 - transitionend: 在 CSS 觸發完成後。

- ### Element.classList
  [參考 MDN](https://developer.mozilla.org/zh-TW/docs/Web/API/Element/classList)
  列出該元素所擁有之類別屬性。
  包含幾種方法：
  - `add( String [, String] )`
    加上類別，若已存在則忽略。
  - `remove( String [,String] )`
    移除類別。
  - `toggle ( String [, force] )`
    若類別不存在則加上，反之則移除。
