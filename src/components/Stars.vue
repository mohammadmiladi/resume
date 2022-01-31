<template>
  <div class="c-stars-plp">
    <span class="c-stars-plp__item"></span>
    <span class="c-stars-plp__item"></span>
    <span class="c-stars-plp__item"></span>
    <span class="c-stars-plp__item"></span>
    <span class="c-stars-plp__item"></span>
    <div class="c-stars-plp__selected" :style="`width:${rate}%;`">
      <span class="c-stars-plp__item"></span>
      <span class="c-stars-plp__item"></span>
      <span class="c-stars-plp__item"></span>
      <span class="c-stars-plp__item"></span>
      <span class="c-stars-plp__item"></span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    rate: {
      default: 0,
      type: Number,
    },
  },
};
</script>

<style scoped>
.c-stars-plp {
  display: flex;
  flex-wrap: nowrap;
  font-size: 20px;
  position: relative;
  direction: ltr;
}
.c-stars-plp__item {
  line-height: 1;
  color: #bbb;
}
*,
::before,
::after {
  background-repeat: no-repeat;
  box-sizing: inherit;
}
.c-stars-plp__selected {
  position: absolute;
  left: 0;
  top: 0;
  direction: ltr;
  display: flex;
  flex-wrap: nowrap;
  overflow: hidden;
}
.c-stars-plp__item:before {
  width: 18px;
  height: 19px;
  background: url(~@/assets/images/b7a76a25.svg) no-repeat 50% 50%;
  background-size: 100%;
  content: "";
  display: inline-block;
}
.c-stars-plp__selected .c-stars-plp__item:before {
  background-image: url(~@/assets/images/d16ba175.svg);
}
</style>
