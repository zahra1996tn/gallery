<template>
  <div class="container">
      <!-- <img v-for="im in image" :key="im" :src="im" class="img"> -->
      <!-- <a> <i class="fa fa-heart"  v-on="$Listener"></i> {{a}} </a> -->
      <img :src="img" class="img">
      <like  @click="like" :a="a"/>
  </div>
</template>

<script>
import like from './like.vue'

export default {
  components: { like },
    name:'images',
    // components:{like },
    props:['img'],
    data(){
        return{
            a:0,
            // image:[
            //     '../assets/3.jpg',
            //     '../assets/4.jpg',
            //     '../assets/2.jpg'
            // ]
        }
    
    },
     methods:{
        like(){
            this.a ++;
            // this.color='red';
        }
    }

}
</script>

<style scoped>
    .img{
        width: 280px;
        height: 200px;
        margin: 20px 10px;
        border-radius: 6px;
        cursor: pointer;
    }
    .box-img{
        width: 280px;
        height: 200px;
    }
</style>