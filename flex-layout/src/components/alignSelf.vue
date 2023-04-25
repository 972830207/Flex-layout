<template>
  <div class="align-self">
    <div class="box">
      <span>align-self </span>
      <div class="box1">
        <div class="one">auto</div>
        <div class="two">flex-start</div>
        <div class="three">flex-end</div>
        <div class="four">center</div>
        <div class="five">baseline </div>
        <div class="six">stretch(默认)</div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="less" scoped>
.align-self {
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
  .box1 {
    display: flex; 
    height: 300px;
    margin: 10px;
    div {
      width: 120px;
      height: 100px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 18px;
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
    .five {
      background: rgba(0, 255, 51, 0.864);
    }
    .six {
      background: rgba(255, 81, 0, 0.797);
    }
  }
  .box1 {
    .one {
      align-self: auto;
    }
    .two {
      align-self: flex-start;
    }
    .three {
      align-self: flex-end;
    }
    .four {
      align-self: center;
    }
    .five {
      align-self: baseline;
    }
    .six {
      align-self: stretch;
      height: auto;
    }
  }
}
</style>
