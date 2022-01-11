<template>
<div>
  <img class="img-bg" src="./assets/template.jpg">
</div>
<div class="box-bold">
  <img src="./assets/2.jpg">
  <img src="./assets/4.jpg">
  <img src="./assets/5.jpg">
  <img src="./assets/6.jpg">
  <img src="./assets/7.jpg">
</div>
<div class="container">
  <gallery :src="img" v-for="img in images" :key="img" class="" />
</div>
</template>

<script>
import gallery from './components/gallery.vue'

export default {
  components: { gallery },
  name: 'App',
  data(){
    return{
        images:[
        "https://s4.uupload.ir/files/3_0jxd.jpg",
        "https://s4.uupload.ir/files/8_blfi.jpg",
        "https://s4.uupload.ir/files/7_5u2y.jpg",
        'https://s4.uupload.ir/files/11_y993.jpg',
        'https://s4.uupload.ir/files/5_7kmw.jpg',
        'https://s4.uupload.ir/files/2_6j5.jpg',

        ],
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: center;
}
.container{
  position: relative;
  margin-top: 140px;
  z-index: 555;
  display: inline-block;
  justify-content: center;
  width: 900px;
  text-align: center;
  /*shadow*/ 
  border-radius: 50px;
  background: #f5f5f5;
  box-shadow: -2px 14px 30px #bebebe, 2px 2px 89px #ffffff;
}
@media(max-width:925px){
  .container{
    width: 100%;
    justify-content: center;
    display: inline-block;
    text-align: center;
    align-items: center;
    margin: 55px auto;
  }
}
.img-bg{
  width: 100%;
}
.box-bold img{
  float: right;
  width: 70px;
  height: 70px;
  margin-right: 66px;
}
.box-bold{
  padding: 13px;
  width: 700px;
  height: 70px;
  justify-content: center;
  display: inline-flex;
  margin: -34px auto;
  border-radius: 4px;
  background: #f5f5f5;
  box-shadow: -9px 4px 50px #bebebe, 1px 16px 13px #ffffff;
  }
  @media(max-width:800px){
    .box-bold{
      width: 79%;
      margin:-60px auto ;

    }
    .box-bold img{
      margin-right: 23px;
    }
  }
  @media(max-width:615px){
    .box-bold{
      display: none;
    }
  }
  @media(max-width:330px){
    .container img{
      width: 210px !important;
      height: 150px !important;
    }
    .img{
      margin-bottom:-28px !important;
    }
  }
</style>
