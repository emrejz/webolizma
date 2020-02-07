<template>
  <div class="customerMainContainer">
    <div>
      <div class="customerTitle">Müşteri Yorumları</div>
      <div v-for="(item, index) in messages" :key="index">
        <div v-if="index === selectedMessage">
          <h2 class="name">
            {{ item.name }}
          </h2>
          <div class="text">
            {{ item.text }}
          </div>
        </div>
      </div>
      <div class="circleBox">
        <div v-for="(item, index) in messages" :key="item.name">
          <span
            :class="{ active: initIndex == index }"
            @click="selectMessage(index)"
            class="circle"
          >
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Customer",
  data: function() {
    return {
      initIndex: 0,
      messages: [
        {
          name: "nazommmmm",
          text:
            "Bir is gezisi sirasinda 1 gece konakladık gayet memnun kaldık kesinlikle tavsiye ediyorum . Odalar temiz fiyati gayet uygun konumu merkezi ve personel gayet ilgili kahvaltısı cok zengin. Biz memnun kaldik. :)"
        },
        {
          name: "TripAdvisor Üyesi",
          text:
            "Ulus bölgesini görünce kesin mutsuz olacağız dedik ama Otel bizi şaşırttı. . Temiz, nezih, personel samimi ve kaliteli bir otel. Odaları biraz küçük olmasına rağmen tavsiye edebilecegim bir otel. Ailenizle de rahatlıkla kalabilirsiniz.."
        },
        {
          name: "Özgür Murat DEMİR",
          text:
            "Yaklaşık 12 senedir bu otelde konakliyoruz. 12 senede hizmet standartlarını değiştirmeden ileri götüren bir otel. Otelin kapısından girdiğiniz anda otel personeli sizi 5 yıldızlı bir otele gelmiş gibi hissettiriyor. Her ile bir asal otel lazim. Aradığınız herşeyi burada bulabilirsiniz."
        },
        { name: "Azi̇z Bahadır AKAR", text: "Teşekkürler gayet güzel." }
      ]
    };
  },
  computed: {
    selectedMessage() {
      return this.initIndex;
    }
  },
  methods: {
    selectMessage(index) {
      this.initIndex = index;
    }
  }
};
</script>

<style scoped>
.active {
  background-color: gray !important;
}
.customerTitle {
  font-size: 32px;
  font-weight: 700;
}
.circle {
  width: 10px;
  height: 10px;
  margin-left: 10px;
  border-radius: 50%;
  background-color: white;
  float: left;
  margin-top: 20px;
}
.circle:hover {
  cursor: pointer;
}
.circleBox {
  width: 100%;
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.customerMainContainer {
  display: flex;
  flex-direction: row;
  width: 100%;
  min-height: 420px;
  padding: 20px 100px;
  background-attachment: fixed;
  background-image: url("../assets/customer-bg.jpg");
  color: white;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
