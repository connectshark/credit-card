<template>
  <div class="circles">
    <div class="circle circle-1"></div>
    <div class="circle circle-2"></div>
  </div>
</template>

<script>
export default {
  name: 'circles'
}
</script>

<style lang="scss" scoped>
.circle{
  position: absolute;
  border-radius: 50%;
  background: radial-gradient(#006db3, #29b6f6);
}
.circles {
  position: absolute;
  height: 270px;
  width: 450px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.circle-1 {
  height: 180px;
  width: 180px;
  top: -50px;
  left: -60px;
}
.circle-2 {
  height: 200px;
  width: 200px;
  bottom: -90px;
  right: -90px;
  opacity: 0.8;
}
</style>
