<template>
  <div id="galery" class="reservationMainContainer">
    <div>
      <div class="rezervTitle">
        Bizimle rezervasyon yaptırdığınızda
      </div>
      <div class="rezervTitle2">En İyi Fiyat Garantisi!</div>
      <div class="rezervTitle3">Online rezervasyon yaptırın veya arayın</div>
      <div class="rezervTitle2"><svg class="svg-inline--fa fa-phone fa-w-16" aria-hidden="true" data-prefix="fas" data-icon="phone" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M493.4 24.6l-104-24c-11.3-2.6-22.9 3.3-27.5 13.9l-48 112c-4.2 9.8-1.4 21.3 6.9 28l60.6 49.6c-36 76.7-98.9 140.5-177.2 177.2l-49.6-60.6c-6.8-8.3-18.2-11.1-28-6.9l-112 48C3.9 366.5-2 378.1.6 389.4l24 104C27.1 504.2 36.7 512 48 512c256.1 0 464-207.5 464-464 0-11.2-7.7-20.9-18.6-23.4z"></path></svg>+90 312 311 55 25</div>
    </div>
    <img class="resImg" src="../assets/res.jpg" />
  </div>
</template>

<script>
export default {
  name: "Reservation"
};
</script>

<style scoped>
  .rezervTitle2 svg{
    width: 42px;
    margin-right: 10px;
  }
  .rezervTitle{
    margin-bottom: 10px;
    font-size: 32px;
    color: #222;
    font-weight: 700;
  }
  .rezervTitle2{
    margin-bottom: 10px;
    font-size: 42px;
    color: #EE4637;
    font-weight: 700;
  }
  .rezervTitle3 {
    margin-bottom: 10px;
    font-size: 24px;
    color: #222;
    font-weight: 700;
  }
.resImg {
  max-width: 50%;
  margin-left: 10px;
  max-height: 100%;
}

.reservationMainContainer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 40px 20px;
  width: 100%;
  height: 100vh;
}
@media (max-width: 500px) {
  .resImg{
    display: none;
  }
  #galery{
    text-align: center;
  }
}
</style>
