<template>
  <div class="card">
    <div class="logo">
      <img src="../assets/visa.png" alt="logo">
    </div>
    <div class="chip">
      <img src="../assets/chip.png" alt="chip">
    </div>
    <div class="number">1234 5678 9012 3456</div>
    <div class="name">SHOUNAK DAS</div>
    <div class="from">10/19</div>
    <div class="to">06/21</div>
    <div class="ring"></div>
  </div>
</template>

<script>
export default {
  name: 'card'
}
</script>

<style lang="scss" scoped>
.card{
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  height: 270px;
  width: 450px;
  border-radius: 25px;
  background-color: rgba(255, 255, 255, 0.2);
  backdrop-filter: blur(30px);
  box-shadow: 0 0 80px rgba(0, 0, 0, 0.2);
  overflow: hidden;
}
img{
  width: 100%;
}
.logo{
  position: absolute;
  width: 50px;
  opacity: 0.8;
  top: 35px;
  right: 40px;
}
.chip{
  position: absolute;
  top: 120px;
  left: 40px;
  width: 50px;
  opacity: 0.8;
}
.number,
.name,
.from,
.to {
  position: absolute;
  color: rgba(255, 255, 255, 0.8);
  font-weight: 400;
  letter-spacing: 2px;
  text-shadow: 0 0 2px rgba(0, 0, 0, 0.6);
}
.number {
  left: 40px;
  bottom: 65px;
  font-family: "Nunito", sans-serif;
}
.name {
  font-size: 0.5rem;
  left: 40px;
  bottom: 35px;
}
.from {
  font-size: 0.5rem;
  bottom: 35px;
  right: 110px;
}

.to {
  font-size: 0.5rem;
  bottom: 35px;
  right: 40px;
}
.ring {
  position: absolute;
  height: 500px;
  width: 500px;
  border-radius: 50%;
  background: transparent;
  border: 50px solid rgba(255, 255, 255, 0.1);
  bottom: -250px;
  right: -250px;
  box-sizing: border-box;
}

.ring::after {
  content: "";
  position: absolute;
  height: 600px;
  width: 600px;
  border-radius: 50%;
  background: transparent;
  border: 30px solid rgba(255, 255, 255, 0.1);
  bottom: -80px;
  right: -110px;
  box-sizing: border-box;
}
</style>
