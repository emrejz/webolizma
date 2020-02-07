<template>
  <div id="home" class="homeMainContainer">
    <img src="../assets/slide1.jpg" />
    <div class="rezervPanel">
      <div class="dates">
        <div class="enterDate">
          <div>
            Giriş Tarihi
          </div>
          <img src="../assets/icon-date.svg" />
        </div>
        <div class="exitDate">
          <div>
            Çıkış Tarihi
          </div>
          <img src="../assets/icon-date.svg" />
        </div>
      </div>
      <div class="selectors">
        <select class="adultSelect">
          <option>Yetişkin Sayısı</option>
          <option>1</option>
          <option>2</option>
          <option>3</option>
          <option>4</option>
        </select>
        <select class="childSelect">
          <option>Çocuk Sayısı</option>
          <option>0</option>
          <option>1</option>
          <option>2</option>
          <option>3</option>
          <option>4</option>
        </select>
      </div>

      <div class="rezervButton">
        REZERVASYON
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style scoped>
.dates {
  flex: 1;
  display: flex;
  flex-direction: row;
}
.selectors {
  flex: 1;
  display: flex;
  flex-direction: row;
}
.enterDate {
  flex: 1;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.exitDate {
  flex: 1;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.rezervPanel {
  box-shadow: 1px 0px 13px 0px black;
  width: 92%;
  height: 60px;
  border-radius: 40px;
  background-color: white;
  display: flex;
  justify-content: space-between;
  overflow: hidden;
  align-items: center;
  position: absolute;
  bottom: 30px;
}
.adultSelect {
  flex: 1;
  border: none;
}
.childSelect {
  flex: 1;
  border: none;
}
.rezervButton {
  background-color: #ee4637;
  color: white;
  padding: 30px;
}
.homeMainContainer {
  /* background-image: url("../assets/slide1.jpg");
       background-repeat: no-repeat;
       background-size: contain; */
  position: relative;
  height: 100vh;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  padding-bottom: 66px;
}
#home {
  height: 100vh;
  overflow: hidden;
}
@media (max-width: 700px) {
  .rezervPanel {
    border-radius: 0px;
    flex-direction: column;
    height: fit-content;
  }
  .dates {
    width: 100%;
  }
  .selectors {
    width: 100%;
  }
  .enterDate {
    padding: 20px;
    margin-right: 8px;
    border: 1px solid #ebebeb;
  }
  .exitDate {
    padding: 20px;
    border: 1px solid #ebebeb;
  }
  .adultSelect {
    padding: 20px;
    margin-right: 8px;
    border: 1px solid #ebebeb;
  }
  .childSelect {
    padding: 20px;
    border: 1px solid #ebebeb;
  }
  .rezervButton {
    margin-top: 20px;
    width: 100%;
    text-align: center;
    padding: 20px;
  }
}
</style>
