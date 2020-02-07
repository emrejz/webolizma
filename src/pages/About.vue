<template>
  <div id="about" class="aboutMainContainer">
    <div class="aboutLeft">
      <img src="../assets/home-about.jpg" />
    </div>
    <div class="aboutRight">
      <h1>ASAL OTEL</h1>
      <div class="description">
        Asal Hotel, 2003 yılından bu yana turizm sektöründe tecrübeli ve
        kaliteli hizmetini, uluslararası çağdaş otelcilik anlayışı, kesintisiz
        değişim ve atılım ilkesiyle birleştirerek modern bir şehir otelinin
        gerektirdiği donanımla profesyonel hizmet vermektedir. Tecrübe,
        profesyonellik ve kaliteli hizmet anlayışımız ile Asal Hotel ailesi
        olarak sizleri ağırlamaktan mutluluk duyarız.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About"
};
</script>

<style scoped>
.description {
  font-size: 14px;
  color: #666;
  line-height: 20px;
}
.aboutMainContainer img {
  max-height: 100%;
}
.aboutMainContainer {
  padding: 40px 20px;
  padding-top: 100px;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 100vh;
  display: flex;
  flex: 1;
}
.aboutLeft {
  padding: 10px;
  flex: 1;
  width: fit-content;
  height: 100%;
}
.aboutRight {
  padding: 10px;
  flex: 1;
}
.aboutMainContainer h1 {
  font-size: 42px;
  color: #222;
  font-weight: 700;
}
@media (max-width: 700px) {
  .aboutMainContainer {
    flex-direction: column;
  }
  .aboutLeft img{
    width: 100%;
  }
  
}
</style>
