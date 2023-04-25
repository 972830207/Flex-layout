<template>
  <div class="align-items">
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
      <span>baseline</span>
      <div class="box4">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
      </div>
    </div>
    <div class="box">
      <span>stretch（默认值）</span>
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
.align-items {
  padding: 2rem;
  display: flex;
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
    height: 200px;
    div {
      width: 50px;
      //   height: 100px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 22px;
      color: white;
      font-weight: bolder;
    }
    .one {
      background: red;
      height: 40px;
    }
    .two {
      background: green;
      height: 80px;
    }
    .three {
      background: blue;
      height: 120px;
    }
    .four {
      background: rgba(98, 0, 255, 0.797);
    }
  }
  .box1 {
    align-items: flex-start;
  }
  .box2 {
    align-items: flex-end;
  }
  .box3 {
    align-items: center;
  }
  .box4 {
    align-items: baseline;
  }
  .box5 {
    align-items: stretch;
  }
}
</style>
