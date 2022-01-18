<template> 
 <h1> گالری تصاویر </h1>
 <h2> در دنیایی که همه چیز خیلی زود فراموش می‌شود،
عکس‌ها سندی هستند که با ثبت یک لحظه،
راوی تاریخ می‌شوند. </h2>
<div class="bg">
  <img src='./assets/36.jpg' class="img-bg">
</div>
<gallery />

</template>

<script>
import gallery from './components/gallery.vue'

export default {
  components: { gallery},
  name: 'App',
  data(){
    return{
    }
  },

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  text-align: center;
  font-family: IS;
}
@font-face{
font-family: IS;
font-style: normal;
src: url("../public/font/IRAN Sans Regular (mmrostami.blog.ir).ttf");
}
h1{
  position: absolute;
    margin: 200px 276px;
    font-size: 41px;
    color: #2c3e50;
}
h2{
  position: absolute;
    margin: 280px 200px;
    font-size: 20px;
    max-width: 300px;
        text-align: right;
    word-spacing: 11px;
}
/* @media(max-width:587px){
  h1{
    margin: 290px 120px;
  }
 
} */
.container{
  justify-content: center;
  text-align: center;
  display: inline-grid;
}


  @media(max-width:330px){
    .container img{
      width: 210px !important;
      height: 150px !important;
      margin-top:-69px;
    }
    .img{
      margin-bottom:-28px !important;
      height: 160px !important;
      border: none !important;
    }
  }
  .bg{
    height: 600px;
    background-color: #fff;
  }
  .img-bg{
    margin-left: 600px;
  }
  @media(max-width:1224px){
    .img-bg{
      margin-left: 550px;
    }
    h1{
      margin: 216px 276px;
    }
  }
   @media(max-width:1175px){
    .img-bg{
      margin-left: 400px;
      width: 500px;
    }
   
  } 
  @media(max-width:1100px){
    h1{
      margin: 216px 200px;
    }
   h2{
     margin: 280px 100px;
   }
  }
  @media(max-width:925px){
    .img-bg{
      margin-left: 320px;
      width: 430px;
    }
    h1{
    margin: 180px 70px;
    }
    h2{
    margin: 250px 20px;
    }
    .bg{
      height: 450px;
    }
  }
  @media(max-width:775px){
    .img-bg{
      margin-left: 250px;
      width: 380px;
    }
  }
  @media(max-width:655px){
    .img-bg{
      margin-left: 200px;
      width: 320px;
    }
    h1{
      margin: 120px 50px;
      font-size:35px ;
    }
    h2{
    margin: 190px 10px;
    }
    .bg{
      height: 400px;
    }
  } 
   @media(max-width:545px){
    .img-bg{
      margin-left: 150px;
      width: 300px;
    }
    h1{
      margin: 120px 30px;
      font-size:32px ;
    }
    h2{
      margin: 190px 0px;
      font-size:19px ;
    }
  }
  @media(max-width:475px){
    .img-bg{
      margin: 0 5px;
      width: 250px;
    }
    h1{
      display: block;
      /* margin: 320px 45px; */
      font-size:32px ;
      justify-content: center;
      align-items: center;
      margin-top: 280px;
    }
    h2{
      margin-top:340px ;
      max-width:250px ;
      text-align: justify !important;
    }
    .bg{
      height: 500px;
    }
  }
  </style>
