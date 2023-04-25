<template>
  <div class="align-content">
    <div class="box">
      <span>flex-start</span>
      <div class="box1">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
    <div class="box">
      <span>flex-end</span>
      <div class="box2">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
    <div class="box">
      <span>center </span>
      <div class="box3">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
    <div class="box">
      <span>space-between </span>
      <div class="box4">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
    <div class="box">
      <span> space-around </span>
      <div class="box5">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
    <div class="box">
      <span>stretch（默认值[2、5未设置宽度]）</span>
      <div class="box6">
        <div class="one">1</div>
        <div class="two">2</div>
        <div class="three">3</div>
        <div class="four">4</div>
        <div class="five">5</div>
        <div class="six">6</div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="less" scoped>
.align-content {
  padding: 2rem;
  display: flex;
  flex-wrap: wrap;
  .box {
    text-align: center;
    font-weight: bold;
    font-size: 18px;
    color: rgba(0, 213, 255, 0.761);
    border: 1px solid #000;
    width: 48%;
    margin: 0.5%;
  }
  .box1,
  .box2,
  .box3,
  .box4,
  .box5,
  .box6 {
    display: flex;
    flex-flow: column wrap;
    height: 130px;
    margin: 10px;
    div {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 22px;
      color: white;
      font-weight: bolder;
      margin: 2px 4px;
    }
    .one {
      background: red;
      width: 100px;
      height: 40px;
    }
    .two {
      background: green; 
      height: 50px;
    }
    .three {
      background: blue;
      width: 100px;
      height: 40px;
    }
    .four {
      background: rgba(98, 0, 255, 0.797);
      width: 300px;
      height: 50px;
    }
    .five {
      background: rgba(0, 255, 51, 0.864);
      height: 20px;
    }
    .six {
      background: rgba(255, 81, 0, 0.797);
      width: 100px;
      height: 40px;
    }
  }
  .box1 {
    align-content: flex-start;
  }
  .box2 {
    align-content: flex-end;
  }
  .box3 {
    align-content: center;
  }
  .box4 {
    align-content: space-between;
  }
  .box5 {
    align-content: space-around;
  }
  .box6 {
    align-content: stretch;
  }
}
</style>
