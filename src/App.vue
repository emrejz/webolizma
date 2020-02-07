<template>
  <div class="app">
    <Navbar />
    <Home/>
    <About/>
    <Rooms/>
    <Reservation/>
    <Info/>
    <Location/>
    <Customer/>
    <Contact/>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './pages/Home.vue'
import About from './pages/About.vue'
import Rooms from './pages/Rooms.vue'
import Reservation from './pages/Reservation.vue'
import Info from './pages/Info.vue'
import Location from './pages/Location.vue'
import Customer from './pages/Customer.vue'
import Contact from './pages/Contact.vue'

export default {
  name: 'app',
  components: {
    Navbar,
    Home,
    About,
    Rooms,
    Reservation,
    Info,
    Location,
    Customer,
    Contact,
  }
}
</script>

<style>
html,body {
  font-family: 'Poppins', sans-serif;
  margin: 0px;
  width: 100%;
  height: 100vh;
  padding: 0px;
  overflow-x: hidden;
  position: relative;
  scroll-behavior: smooth;
}
.app{
  width: 100%;
  height: max-content;
  position: relative;
}
* {
  box-sizing: border-box;
}
::-webkit-scrollbar{
  width: 0px;
}
</style>
