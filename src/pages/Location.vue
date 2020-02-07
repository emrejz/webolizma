<template>
  <div id="location" class="locationMainContainer">
    <h1>ÖNEMLİ LOKASYONLAR</h1>

    <div class="locationImgs">
      <div class="slide1">
        <div class="slideTitle">Kültür Sanat</div>
        <img class="lg" src="../assets/local-1.jpg" />
      </div>
      <div class="slide2">
        <div class="slideTitle">Ulaşım</div>

        <img class="sm" src="../assets/transport.jpg" />
      </div>
    </div>
    <div class="locationImgs">
      <div class="slide2">
        <div class="slideTitle">Hastaneler</div>

        <img class="sm" src="../assets/hospital.jpg" />
      </div>

      <div class="slide1">
        <div class="slideTitle">Spor</div>

        <img class="lg" src="../assets/sport.jpg" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Location"
};
</script>

<style scoped>
.slide1 {
  position: relative;
  display: flex;
  overflow: hidden;
  flex: 2;
  cursor: pointer;
}
.slide2 {
  position: relative;
  overflow: hidden;
  display: flex;
  flex: 1;
  cursor: pointer;
}
.slide1:hover img {
  background-blend-mode: rgba(255, 255, 255, 0.3);
}
.slideTitle {
  position: absolute;
  bottom: 18px;
  left: 10px;
  color: white;
  font-size: 24px;
  font-weight: 700;
}
.locationImgs img {
  width: -webkit-fill-available;
  margin: 4px;
  border-radius: 10px;
}
.locationImgs {
  width: 100%;
  height: 450px;
  display: flex;
  flex-direction: row;
  flex: 1;
}

.locationMainContainer {
  flex: 1;
  display: flex;
  flex-direction: column;
  padding: 40px 20px;
  width: 100%;
  overflow: hidden;
  height: fit-content;
}
</style>
