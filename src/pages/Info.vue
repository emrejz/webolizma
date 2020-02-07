<template>
  <div class="infoMainContainer">
    <div class="infoTitle">OTEL BİLGİSİ</div>
    <div class="infoIcons">
      <div class="infoCard">
        <img src="../assets/icon-entery.svg" />
        <div>Giriş Saati: 14:00</div>
        <div>Çıkış Saati: 12:00</div>
      </div>
      <div class="infoCard">
        <img src="../assets/icon-breakfast.svg" />
        <div>Ekspres Kahvaltı</div>
      </div>
      <div class="infoCard">
        <img src="../assets/icon-clean.svg" />
        <div>Kuru Temizleme</div>
      </div>
      <div class="infoCard">
        <img src="../assets/icon-smoke.svg" />
        <div>Sigara İçilen / İçilmeyen Oda</div>
      </div>
      <div class="infoCard">
        <img src="../assets/icon-park.svg" />
        <div>Otopark</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Info"
};
</script>

<style scoped>
.infoTitle {
  color: #222;
  font-size: 32px;
  font-weight: 700;
}
.infoMainContainer {
  padding: 40px 20px;
  width: 100%;
  height: 100%;
  background-color: white;
}
.infoIcons {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
.infoCard {
  text-align: center;
  background: #fbfbfb;
  padding: 40px;
  margin: 8px;
  cursor: pointer;
  font-size: 14px;
  color: #333;
  font-weight: 700;
}
.infoCard:hover {
  box-shadow: 0 0 20px gray;
  color: #ee4637;
}
.infoCard div:nth-child(even) {
  width: 100px;
  margin-top: 8px;
}
</style>
