<template>
  <footer class="footerMainContainer">
    <div class="firstRow">
      <img src="../assets/card-icon.png" />
      <span>© 2019 Asal Hotel - Tüm Hakları Saklıdır.</span>
    </div>
    <img src="../assets/webolizma.png" />
  </footer>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style scoped>
.footerMainContainer {
  min-height: 125px;
  padding: 0 20px;
  position: absolute;
  left: 0;
  bottom: 0;
  right: 0;
  z-index: 10;
  width: 100%;
  background-color: #343434;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.firstRow {
  margin-top: 40px;
  margin-bottom: 20px;
  display: flex;
  width: 100%;
  justify-content: space-between;
  color: #6b6b6b;
  font-size: 12px;
  align-items: flex-end;
}
@media (max-width: 500px) {
  .firstRow {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
