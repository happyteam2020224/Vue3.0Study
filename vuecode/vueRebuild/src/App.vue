<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
$(function(){
    // 解决chrome的图片选中问题
    function imgdragstart(){return false;}
    console.log(document.images);
    try
    {
    for(let i in document.images)document.images[i].ondragstart=imgdragstart; 
    }catch(e){

    }
});
</script>

<style>
#app {
 width: 100%;
 height: 100%;
-webkit-user-select: none;
-moz-user-select: none;
-o-user-select: none;
user-select: none;
  }

</style>

