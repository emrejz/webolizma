<template>
  <div id="room" class="roomsMainContainer">
    <h1>ODALAR</h1>
    <div class="roomsDesc">
      50 Standart oda, 8 Exclusive oda olmak üzere toplam 58 oda ile hizmet
      vermekteyiz.
    </div>
    <div class="roomsImg">
      <div class="roomCard">
        <img src="../assets/singleroom.jpg" />
        <div class="roomCardDesc">
          <div>
            Single Room
          </div>
          <div>
            1 ADET ÇİFT KİŞİLİK YATAK
          </div>
          <div>INCELE</div>
        </div>
      </div>
      <div class="roomCard">
        <img src="../assets/double-room.jpg" />
        <div class="roomCardDesc">
          <div>
            Double Room
          </div>
          <div>
            1 ADET ÇİFT KİŞİLİK YATAK
          </div>
          <div>
            1 ADET TEK KİŞİLİK YATAK
          </div>
          <div>INCELE</div>
        </div>
      </div>
      <div class="roomCard">
        <img src="../assets/family_room.jpg" />
        <div class="roomCardDesc">
          <div>
            Family Room
          </div>
          <div>
            1 ADET ÇİFT KİŞİLİK YATAK
          </div>
          <div>
            2 ADET TEK KİŞİLİK YATAK
          </div>
          <div class="roomButton">INCELE</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Rooms"
};
</script>

<style scoped>
.roomsMainContainer h1 {
  font-size: 32px;
  color: #222;
  font-weight: 700;
}
.roomsImg {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
.roomCard {
  cursor: pointer;
  position: relative;
  transition: 1s ease;
  box-shadow: 0px 0px 16px 1px gray;
  border-radius: 10px;
  max-width: fit-content;
  max-height: fit-content;
  margin-top: 20px;
  overflow: hidden;
}
.roomCardDesc {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  bottom: 0;
  left: 0;
  right: 0;
  flex-direction: column;
  color: white;
}
.roomCardDesc div:first-child {
  font-size: 24px;
  margin-bottom: 10px;
}
.roomCardDesc div:last-child {
  background-color: #ee4637;
  padding: 10px 30px;
  border-radius: 20px;
  margin-bottom: 24px;
  margin-top: 10px;
}
.roomCard img {
  max-width: 100%;
}
.roomCard:hover {
  transform: scale(1.05);
}
.roomCard:hover .roomButton {
  background-color: #343434;
}
.roomsDesc {
  text-align: center;
  font-size: 18px;
  color: #222;
  font-weight: 700;
  margin-bottom: 20px;
}
.roomsMainContainer {
  padding: 40px 20px;
  width: 100%;
  height: 100%;
}
</style>
