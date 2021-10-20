# CSS Variable

## HTML

- ### input
  [詳細可參考 MDN](https://developer.mozilla.org/zh-TW/docs/Web/HTML/Element/input)
  ```html
  // Example:
  <input
    id="spacing"
    type="range"
    name="spacing"
    value="10"
    min="10"
    max="200"
    data-sizing="px"
  />
  ```
  - #### type
  1. 根據"type"去定義;若 type 為定義則為"text"。
  2. 此次用到的 type:
     (1) range：數值，可以定義範圍，來排除不需要的數值。
     (2) color：顏色選取。
  - #### value
    為 input 的初始值。

---

# CSS

- ### 變數

1. 定義變數，可以針對整個 html，並加上'--'

```css
// Example:
:root {
  --base: #ffc600;
  --spacing: 10px;
  --blur: 5px;
}
```

2. 取用變數，需加上 var()

```css
// Example:
img {
  padding: var(--spacing);
  background: var(--base);
  filter: blur(var(--blur));
}
```

---

# JS

- ### setProperty

```js
object.setProperty(propertyName, value);
```

可以用來設置和改變物件的屬性。
在這裡是改變 CSS，所已要寫成`object.style.setProperty()`

- ### addEventListener

1. 可以根據接收到的 event 去做進一步的觸發。
   [Event Type 參考 MDN](https://developer.mozilla.org/en-US/docs/Web/Events)
2. 此次用到的 event:
   (1) change：內容改變。
   (2) mousemove：滑鼠移動。
