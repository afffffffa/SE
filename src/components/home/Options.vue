<template>
  <div class="container">
    <div class="card">
      <div class="personal-info">
        <div class="avatar">
          <img src="@/assets/img/ad.png" alt="avatar">
        </div>
        <div class="info">
          <h3>{{ personName }}</h3>
          <p>ID: {{ personID }}</p>
          <p>余额: {{ balance }}</p>
        </div>
      </div>
      <div class="buttons">
        <button type="button" class="btn1" @click="chooseShop">点单</button>
        <button type="button" class="btn2" @click="chooseShop">送餐单</button>
      </div>
    </div>
    <!--    <img src="@/assets/img/ad2.png" class="advertisement">-->
  </div>
</template>

<script>
export default {
  name: 'Options',
  data() {
    return {
      personName: '张三',
      personID: '00001',
      balance: 100.0
    }
  },
  methods: {
    chooseShop(){
      this.$router.push('/chooseshop');
    }
  }
}
</script>

<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  bottom: 90px;
}
.card {
  width: 80%;
  height: 80%;
  margin: auto;
/*  background-color: rgba(255, 255, 255, 0.8);：设置背景颜色为白色，透明度为0.8。*/
/*  border-radius: 20px;：设置圆角半径为20像素。*/
/*box-shadow: 0px 5px 10px rgba(0,0,0,0.2);：设置阴影效果，阴影偏移量为0像素水平、5像素垂直，阴影模糊度为10像素，阴影颜色为黑色，透明度为0.2。*/
/*  display: flex;：设置为Flex布局。*/
/*flex-direction: column;：设置子元素排列方向为垂直方向。*/
/*justify-content: center;：设置子元素在主轴方向上居中对齐。*/
/*align-items: center;：设置子元素在交叉轴方向上居中对齐。*/
/*padding: 30px;：设置内边距为30像素。*/
  background-color: rgba(255, 255, 255, 0.8);
  border-radius: 20px;
  box-shadow: 0px 5px 10px rgba(0,0,0,0.2);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  /*align-items: center;*/
  padding: 30px;
}
.personal-info {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}
.avatar {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  overflow: hidden;
  margin-right: 20px;
}
.avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.info h3 {
  font-size: 32px;
  font-weight: bold;
  margin-top: 0;
  margin-bottom: 10px;

}
.info p {
  font-size: 20px;
  margin: 0;
}
.buttons {
  display: flex;
  justify-content: space-between;
}
.btn1, .btn2 {
  width: 80%;
  height: 100px;
  border: none;
  /*cursor: pointer;*/

  font-size: 30px;
  border-radius: 10px;
  margin: 0 10px;
}
.btn1 {
  color: #fff;
  background-image: url(../../assets/img/swipe/swipe1.jpg);
  background-size: cover;
}
.btn2 {color: #110011;

  background-image: url(../../assets/img/swipe/swipe2.jpg);
  background-size: cover;
}
/*.advertisement {*/
/*  left: 50%;*/
/*  transform: translateX(-50%);*/
/*  width: 50%;*/
/*  height: 30%;*/
/*  position: relative;*/
/*  bottom: 90px;*/
/*}*/
</style>
