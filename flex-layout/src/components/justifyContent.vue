<template>
  <div class="justify-content">
    <div class="box">
      <span>flex-start</span>
      <div class="box1">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>flex-end</span>
      <div class="box2">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>center</span>
      <div class="box3">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>space-between</span>
      <div class="box4">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>space-around</span>
      <div class="box5">
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
.justify-content {
  padding: 2rem; 
  .box {
    text-align: center;
    font-weight: bold;
    font-size: 18px;
    color: rgba(0, 213, 255, 0.761);
    border: 1px solid #000;
  }
  .box1,
  .box2,
  .box3,
  .box4,
  .box5 {
    display: flex; 
    margin: 10px;
    div {
      width: 100px;
      height: 50px;
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
    justify-content: flex-start;
  }
  .box2 {
    justify-content: flex-end;
  }
  .box3 {
    justify-content: center;
  }
  .box4 {
    justify-content: space-between;
  }
  .box5 {
    justify-content: space-around;
  }
}
</style>
