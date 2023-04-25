<template>
  <div class="order">
    <div class="box">
      <span>order:0213</span>
      <div class="box1">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>order:2130</span>
      <div class="box2">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>order:3210</span>
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
.order {
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
    .one {
      order: 0;
    }
    .two {
      order: 2;
    }
    .three {
      order: 1;
    }
    .four {
      order: 3;
    }
  }
  .box2 {
    .one {
      order: 2;
    }
    .two {
      order: 1;
    }
    .three {
      order: 3;
    }
    .four {
      order: 0;
    }
  }
  .box3 {
    .one {
      order: 3;
    }
    .two {
      order: 2;
    }
    .three {
      order: 1;
    }
    .four {
      order: 0;
    }
  }
}
</style>
