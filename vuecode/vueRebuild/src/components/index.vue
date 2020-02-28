<template>
  <div class="container">
        <audio id='audio_1' src='../static/iamge/Audio/Loading_BGM.mp3' muted></audio>
        <audio id='audio_3' src='../static/iamge/Audio/Selected.wav' muted></audio>
        <!-- <video  src="../assets/iamge/active-Image/panda_video/question1/q1.mp4"></video> -->
        <!-- logo和按钮 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/logo.png" id="firstpage1">
        <img :src="logo_btn?require('../assets/iamge/pandaImage/firstPage_firework/button_star.png'):require('../assets/iamge/pandaImage/firstPage_firework/button_star_enter (1).png')" id="firstpage2"   @mouseup="$router.push('/content')" @mouseenter="logo_btn=false;playMusic('start')" @mouseleave="logo_btn=true">
        <!-- 三个小精灵 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/bluespirit.png" id="firstpage3">
        <img src="../assets/iamge/pandaImage/firstPage_firework/orangespirit.png" id="firstpage4">
        <img src="../assets/iamge/pandaImage/firstPage_firework/greenspirit.png" id="firstpage5">
        <!-- 熊猫 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/panda_1.png" id="firstpage6">
        <img src="../assets/iamge/pandaImage/firstPage_firework/panda_3.png" id="firstpage7">
        <img src="../assets/iamge/pandaImage/firstPage_firework/panda_2.png" id="firstpage8">
        <!-- 石头 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/stone_1.png" id="firstpage9">
        <img src="../assets/iamge/pandaImage/firstPage_firework/stone_2.png" id="firstpage10">
        <!-- 草丛 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/grass_1.png" id="firstpage11">
        <img src="../assets/iamge/pandaImage/firstPage_firework/grass_2.png" id="firstpage12">
        <img src="../assets/iamge/pandaImage/firstPage_firework/grass_2.png" id="firstpage12_2">
        <img src="../assets/iamge/pandaImage/firstPage_firework/grass_3.png" id="firstpage13">
      
        <!-- 花朵 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/flower_1.png" id="firstpage14">
        <img src="../assets/iamge/pandaImage/firstPage_firework/flower_2.png" id="firstpage15">
        <!-- 兔子 -->
        <img src="../assets/iamge/pandaImage/firstPage_firework/rabbit_1.png" id="firstpage16">
        <img src="../assets/iamge/pandaImage/firstPage_firework/rabbit_2.png" id="firstpage17">
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      logo_btn:true,
    }
  },
   mounted: function () {


  },
  methods:{
     playMusic(type){
        type=='start'?document.getElementById("audio_3").play():''
     }
  }
}


</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
html,body {
   width:100%;
   height:100%;
   overflow: hidden;
}
</style>

<style scoped>
.container {
   width:100%;
   height:100%;
   background-image: url('../assets/iamge/pandaImage/firstPage_firework/rise_panda.png');
   background-repeat: no-repeat;
   background-size:100% 100%;
   background-position:center center;
   position: relative;
   overflow: hidden;
}

/* 首页元素位置 */
#firstpage1 {
   position: absolute;
   top: 30px;
   left: 610px;
   z-index: 12;
}

#firstpage2 {
   position: absolute;
   left: 722px;
   top: 625px;
}


#firstpage3 {
   position: absolute;
   left: 50px;
   top:280px;
}
#firstpage4 {
   position: absolute;
   right:77px;
   top:317px;
}
#firstpage5 {
   position: absolute;
   right:0;
   top:590px;
   z-index: 10;
}
#firstpage6 {
   position: absolute;
   left:230px;
   top:75px;
   z-index: 1;
}
#firstpage7 {
   position: absolute;
   left:320px;
   top:561px;
   z-index: 10;
}
#firstpage8 {
   position: absolute;
   right: 230px;
   top:490px;
}
#firstpage9 {
   position: absolute;
   left:0;
   top:810px;
   z-index: 10;
}
#firstpage10 {
   position: absolute;
   right:0;
   top:800px;
   z-index: 2;
}
#firstpage11 {
   position: absolute;
   right:600px;
   top:850px;
}
#firstpage12 {
   position: absolute;
   left:-35px;
   top:669px;
   z-index: 2;
}
#firstpage12_2 {
   position: absolute;
   right: 17px;
   top:702px;
}
#firstpage13 {
   position: absolute;
   right: 0;
   bottom: 10px;
   
}
#firstpage14 {
   position: absolute;
   left:211px;
   bottom: 68px;
   z-index: 3;
   
}
#firstpage15 {
   position: absolute;
   right: 300px;
   bottom: 5px;
   
}
#firstpage16 {
   position: absolute;
   left:250px;
   top:508px;
   
}

#firstpage17 {
   position: absolute;
   left:115px;
   top:520px;
   
}
</style>

