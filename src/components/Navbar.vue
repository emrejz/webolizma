<template>
  <nav class="navbarMainContainer">
    <div class="navbarTopInfo">
      <svg
        class="svg-inline--fa fa-map-marker-alt fa-w-12"
        aria-hidden="true"
        data-prefix="fas"
        data-icon="map-marker-alt"
        role="img"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 384 512"
        data-fa-i2svg=""
      >
        <path
          fill="currentColor"
          d="M172.268 501.67C26.97 291.031 0 269.413 0 192 0 85.961 85.961 0 192 0s192 85.961 192 192c0 77.413-26.97 99.031-172.268 309.67-9.535 13.774-29.93 13.773-39.464 0zM192 272c44.183 0 80-35.817 80-80s-35.817-80-80-80-80 35.817-80 80 35.817 80 80 80z"
        ></path>
      </svg>
      <span>
        Çankırı Caddesi No: 29 06030 Ulus / ANKARA - TÜRKİYE
      </span>
      <svg
        class="svg-inline--fa fa-phone fa-w-16"
        aria-hidden="true"
        data-prefix="fas"
        data-icon="phone"
        role="img"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 512 512"
        data-fa-i2svg=""
      >
        <path
          fill="currentColor"
          d="M493.4 24.6l-104-24c-11.3-2.6-22.9 3.3-27.5 13.9l-48 112c-4.2 9.8-1.4 21.3 6.9 28l60.6 49.6c-36 76.7-98.9 140.5-177.2 177.2l-49.6-60.6c-6.8-8.3-18.2-11.1-28-6.9l-112 48C3.9 366.5-2 378.1.6 389.4l24 104C27.1 504.2 36.7 512 48 512c256.1 0 464-207.5 464-464 0-11.2-7.7-20.9-18.6-23.4z"
        ></path>
      </svg>
      <span>
        +90 312 311 55 25
      </span>
      <span>TR</span>
    </div>
    <div class="navbarContainer">
      <img src="../assets/asal-hotel-logo.png" />
      <a href="#home">anasayfa</a>
      <a href="#about">hakkımızda</a>
      <a href="#room">odalar</a>
      <a href="#galery">galeri</a>
      <a href="#location">önemli lokasyonlar</a>
      <a href="#contact">iletişim</a>
    </div>
    <img class="hamburgerMeu" src="../assets/menu.png" />
  </nav>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style scoped>
.hamburgerMeu {
  display: none;
}
.navbarMainContainer svg {
  color: #ee4637;
  width: 14px;
  margin-right: 10px;
  margin-left: 20px;
}
.navbarMainContainer {
  height: 140px;
  border-bottom: 1px solid white;
  padding: 0 20px;
  position: absolute;
  color: white;
  z-index: 10;
  width: 100%;
}
.navbarContainer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.navbarTopInfo {
  display: flex;
  justify-content: flex-end;
  padding-top: 10px;
  padding-bottom: 30px;
}
.navbarMainContainer img {
  margin-right: 100px;
}
.navbarMainContainer a {
  text-transform: uppercase;
  color: white;
  text-decoration: none;
  padding-bottom: 26px;
  transition: 1s ease;
}
.navbarMainContainer a:hover {
  border-bottom: 2px solid #ee4637;
  padding-bottom: 48px !important;
}
@media (max-width: 1000px) {
  .navbarMainContainer {
    justify-content: center;
    align-items: center;
    display: flex;
    height: 60px;
    background-color: rgba(0, 0, 0, 0.7);
  }
  .navbarMainContainer a {
    padding: 24px;
  }
  .navbarMainContainer a:hover {
    padding-bottom: 10px !important;
  }
  .navbarContainer {
    width: 90%;
  }
  .navbarTopInfo {
    display: none;
  }
  .navbarMainContainer img {
    display: none;
  }
}
@media (max-width: 760px) {
  .hamburgerMeu {
    display: block !important;
    max-width: 100%;
    position: absolute;
    right: 60px;
    padding: 8px;
    cursor: pointer;
    margin-right: 0px !important;
    background-color: black;
  }
  .navbarContainer {
    display: none;
  }
}
</style>
