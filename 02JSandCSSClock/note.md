# JS and CSS Clock Note

## HTML

- 試著將一個時鐘，寫成三個地區的時鐘。
- 分成名稱區和時鐘圖區。

---

## CSS

1. 若要讓元素水平排列，在父元素加上
   ```css
   display: flex;
   ```
2. 使用`rotate( )`將元素旋轉(2D)

   - 在 style 區塊中

   ```css
   .hand {
     transform: rotate(10deg);
   }
   // 在此處的deg表示旋轉的度數，正數為順時針旋轉，負數為逆時針旋轉。
   ```

   - 在 JS 中

   ```javascript
   const testObj = document.querySelector(".hand");
   testObj.style.transform = "rotate(10deg)";
   ```

3. CSS 應用

   ```css
   position: absolute;
   top: 50%;
   // 物件旋轉的軸心，預設為物件中點(50%),此為最右端(100%)
   transform-origin: 100%;
   transform: rotate(90deg);
   transition: all 0.05s;
   // 變化方式
   transition-timing-function: cubic-bezier(0.1, 2.7, 0.58, 1);
   ```

   - transition-timing-function：[根據貝茲曲線調整變化方式參考 MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)

4. 圖層位置
   用數字排列圖層，數字越大越上層。

```css
p {
  z-index: 1;
}
```

---

## JS

1. `setInterval( )`
   設定固定間隔時間(單位：毫秒)的事件循環。
   例如：

   ```javascript
   setInterval(function1, 1000);
   ```

   每間隔一秒，即運行一次 function1。

2. `Date()`
   時間函數，可取得當下的時間。
