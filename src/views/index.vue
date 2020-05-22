<template>
  <div class="tree-bg">
    <img class="head-img" src="../static/image/headImg.jpg" alt="">
    <div class="energy-list">
      <a href="##" class="energy-item"><span class="text">跑步</span></a>
      <a href="##" class="energy-item active"><span class="text">尤克里里</span></a>
      <a href="##" class="energy-item"><span class="text">跑步</span></a>
      <a href="##" class="energy-item"><span class="text">跑步步</span></a>
      <a href="##" class="energy-item"><span class="text">跑步</span></a>
      <a href="##" class="energy-item"><span class="text">跑步</span></a>
    </div>
    <img class="tree-img" src="../static/image/img1.png" alt="">
  </div>
</template>
<script>
export default {
  data(){
    return{
    }
  }
}
</script>
<style lang="less" scoped>
.energy-list{
  position: absolute;
  top: 80px;
  left:0;
  width: 100%;
  height: 140px;
  // border: 1px solid pink;
  box-sizing: border-box;
}
.energy-item{
  position: absolute;
  top:50px;
  left:50px;
  display:flex;
  align-items: center;
  justify-content: center;
  width:40px;
  height:40px;
  padding:0 5px;
  box-sizing: border-box;
  background: #2bbf2b;
  border-radius: 50%;
  color:#fff;
  font-size: 10px;
  text-decoration: none;
  text-align: center;
  &.active{    
    background: rgba(75,184,16,0.5);
  }
  &:nth-child(1){
    left: 8%;
    top: 78px;
  }
  &:nth-child(2){
    left: 18%;
    top: 22px;
  }
  &:nth-child(3){
    left: 82%;
    top: 55px;
  }
  &:nth-child(4){
    left: auto;
    right: 21%;
    top: 15px;
  }
  &:nth-child(5){
    left: 48%;
    top: 0px;
  }
  &:nth-child(6){
    left: 34%;
    top: 57px;
  }
}
.tree-bg{
  position: absolute;
  width:100%;
  height: 100%;
  .tree-img{
    position:absolute;
    bottom:50px;
    width:100%;
    height:auto;    
    transition: All 0.2s ease-in-out;
  }
  .tree-img.active{
    transform: scale(1.02);
  }
}
.head-img{
  position: absolute;
  top:10px;
  left:10px;
  width:45px;
  height:45px;
  border-radius: 50%;
  border:2px solid #FF9800;
}
</style>
