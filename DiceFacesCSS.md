# CSS/HTML script for the dice faces
- [Source](https://medium.com/better-programming/creating-dice-in-flexbox-in-css-a02a5d85e516)
## CSS
```
.first-face {
  display: flex;
  justify-content: center;
  align-items: center;
}
.dice {
  padding: 4px;
  background-color: tomato;
  width: 104px;
  height: 104px;
  border-radius: 10%;
  margin-right : 10px;
}
.dot{
  display: block;
  width: 24px;
  height: 24px;
  border-radius: 50%;
  background-color:white;
}

.second-face{
  display: flex ;
  justify-content: space-between;
}

.second-face .dot:nth-of-type(2) {
  align-self: flex-end;
}

.third-face {
  display: flex;
  justify-content: space-between;
}

.third-face .dot:nth-of-type(1) {
  align-self :flex-end;
}

.third-face .dot:nth-of-type(2) {
  align-self :center;
}

.fourth-face , .sixth-face, .fifth-face{
  display: flex;
  justify-content: space-between;
}

.fourth-face .column , .sixth-face .column, .fifth-face .column{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.fifth-face .column:nth-of-type(2) {
  justify-content: center;
}
```
# HTML
```
<div class="dice first-face">
  <span class="dot">
  </span>
</div>

<div class="dice second-face">
  <span class="dot">
  </span>
  <span class="dot">
  </span>
</div>

<div class="dice third-face">
  <span class="dot"></span>
  <span class="dot"></span>
  <span class="dot"></span>
</div>

<div class="fourth-face dice">
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
  </div>
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
  </div>
</div>
<div class="fifth-face dice">
  
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
  </div>
  
  <div class="column">
    <span class="dot"></span>
  </div>
  
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
  </div>

</div>
<div class="sixth-face dice">
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
    <span class="dot"></span>
  </div>
  <div class="column">
    <span class="dot"></span>
    <span class="dot"></span>
        <span class="dot"></span>
  </div>

</div>
```