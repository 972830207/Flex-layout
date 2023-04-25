<template>
  <div class="index">
    <div class="line">flex-direction</div>
    <flexDirection />
    <div class="line">flex-wrap</div>
    <flexWrap />
    <div class="line">justify-content</div>
    <justifyContent />
    <div class="line">align-items</div>
    <alignItems />
    <div class="line">align-content(设置row)</div>
    <alignContentRow />
    <div class="line">align-content(设置column)</div>
    <alignContentColumn />
    <div class="line">order</div>
    <order />
    <div class="line">flex</div>
    <flex />
    <div class="line">alignSelf</div>
    <alignSelf />
  </div>
</template>

<script setup lang="ts">
import flexDirection from "../components/flexDirection.vue";
import flexWrap from "../components/flexWrap.vue";
import justifyContent from "../components/justifyContent.vue";
import alignItems from "../components/alignItems.vue";
import alignContentRow from "../components/alignContentRow.vue";
import alignContentColumn from "../components/alignContentColumn.vue";
import order from "../components/order.vue";
import flex from "../components/flex.vue";
import alignSelf from "../components/alignSelf.vue";
</script>

<style lang="less" scoped>
.index {
  .line {
    width: 100%;
    height: 1px;
    background: #000;
    color: rgba(193, 10, 53, 0.714);
    font-size: 24px;
    font-weight: bolder;
    margin: 1rem 0;
  }
}
</style>
