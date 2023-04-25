<template>
  <div class="flex">
    <div class="box">
      <span>flex:0（0 1 0%）</span>
      <div class="box1">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>flex:1（1 1 0%）</span>
      <div class="box2">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>flex:none（0 0 auto）</span>
      <div class="box3">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="less" scoped>
.flex {
  padding: 2rem;
  display: flex;
  .box {
    text-align: center;
    font-weight: bold;
    font-size: 18px;
    color: rgba(0, 213, 255, 0.761);
    border: 1px solid #000;
    margin: 2px;
  }
  .box1,
  .box2,
  .box3 {
    display: flex;
    width: 300px;
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
    .four {
      background: rgba(98, 0, 255, 0.797);
    }
  }
  .box1 {
    div {
      flex: 0;
    }
  }
  .box2 {
    div {
      flex: 1;
    }
  }
  .box3 {
    div {
      flex: none;
    }
  }
}
</style>
