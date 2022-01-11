<template>
<div class="img">
    <img :src="src" :style="styleimg" />
        <i class="fa fa-heart-o" :style="{color:color }" @click="like"></i>  {{ a }}
</div>
</template>

<script>
export default {
    name:'gallery',
    props:['src'],
    data(){
        return{
           a:0,
           styleimg:{
               width:'250px',
               height:'210px'
           }
        }
    },
    methods:{
        like(){
            this.a ++;
            this.color='red';
        }
    }
}
</script>

<style>

body{
    background:#eee;
}
.img{
    float: right;
    margin: 10px 23px;
    padding: 32px 0;
}
.img-head{
    margin: 10px;
    width: 250px;
}
i{
    cursor: pointer;
    display: block !important;
}
</style>