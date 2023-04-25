<template>
  <div class="flex-direction">
    <div class="box">
      <span>row</span>
      <div class="box1">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
      </div>
    </div>
    <div class="box">
      <span>row-reverse</span>
      <div class="box2">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
      </div>
    </div>
    <div class="box">
      <span>column</span>
      <div class="box3">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
      </div>
    </div>
    <div class="box">
      <span>column-reverse</span>
      <div class="box4">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="less" scoped>
.flex-direction {
  padding: 2rem;
  display: flex;
  .box {
    text-align: center;
    font-weight: bold;
    font-size: 18px; 
    color: rgba(0, 213, 255, 0.761);
  }
  .box1,
  .box2,
  .box3,
  .box4 {
    display: flex;
    margin: 10px;
    div {
      width: 100px;
      height: 100px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 22px;
      color: white;
      font-weight: bolder;
    }
    .one {
      background: red;
    }
    .two {
      background: green;
    }
    .three {
      background: blue;
    }
  }
  .box1 {
    flex-direction: row;
  }
  .box2 {
    flex-direction: row-reverse;
  }
  .box3 {
    flex-direction: column;
  }
  .box4 {
    flex-direction: column-reverse;
  }
}
</style>
