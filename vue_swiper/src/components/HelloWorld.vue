<template>
  <swiper :options="swiperOption" ref="mySwiper">
      <swiper-slide v-for="x in msg"><img :src="x" alt=""></swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>  
  </swiper>
</template>

<script>
var info=[
"http://tupian.enterdesk.com/2014/xll/03/04/2/shaosiming3.jpg",
"http://tupian.enterdesk.com/2014/xll/03/03/3/xuenv7.jpg",
"http://up.enterdesk.com/edpic_source/d3/71/6a/d3716a6706c6964904702479543fd945.jpg",
"http://img1.imgtn.bdimg.com/it/u=3957798471,3142624376&fm=27&gp=0.jpg"
]
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: info,
      swiperOption:{
        autoplay: 300,
        loop:true,
        pagination:".pagination"
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
.swiper-container {
  width: 100%;
  height: 60%;
}
img{
  width: 100%;
  height: 60%;
}
</style>
