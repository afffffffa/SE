<template>
  <div>
  	<NavBar>
  		<div slot="nav-text" class="chos-nav"><span @click="backTo" class="glyphicon glyphicon-chevron-left">  </span><p>定位</p></div>
  	</NavBar>
    <div class="cards-item">
      <ul id="myTab" class="nav nav-tabs">
        <li class="active">
          <a href="#location" data-toggle="tab">所有食堂 <span class="glyphicon glyphicon-search"></span></a>
        </li>

      </ul>

      <div class="tab-pane fade in active" id="location">
        <Cards>
          <span slot="shopName">湖畔餐厅</span>
          <span slot="shopDist">2.1KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学湖畔餐厅</p>
          <span class="glyphicon glyphicon-heart-empty starshop" slot="ifstar"></span>
        </Cards>

        <Cards>
          <span slot="shopName">教师餐厅</span>
          <span slot="shopDist">4.1KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学教师餐厅</p>
          <span class="glyphicon glyphicon-heart-empty starshop" slot="ifstar"></span>
        </Cards>

        <Cards>
          <span slot="shopName">茶餐厅</span>
          <span slot="shopDist">4.8KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学茶餐厅</p>
          <span class="glyphicon glyphicon-heart-empty starshop" slot="ifstar"></span>
        </Cards>

        <Cards>
          <span slot="shopName">新生餐厅</span>
          <span slot="shopDist">3.9KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学新生餐厅</p>
          <span class="glyphicon glyphicon-heart-empty starshop" slot="ifstar"></span>
        </Cards>

        <Cards>
          <span slot="shopName">荔园餐厅</span>
          <span slot="shopDist">6.1KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学荔园餐厅</p>
          <span class="glyphicon glyphicon-heart-empty starshop" slot="ifstar"></span>
        </Cards>
        <Cards>
          <span slot="shopName">欣园餐厅</span>
          <span slot="shopDist">8.2KM</span>
          <p slot="shopLocation">广东省深圳市南方科技大学欣园餐厅</p>
          <span class="glyphicon glyphicon glyphicon-heart starshop" slot="ifstar"></span>
        </Cards>
      </div>


    </div>

  </div>
  </div>
</template>

<script>
import NavBar from '@/components/common/NavBar'
import Cards from '@/components/home/options/Cards'

export default {
  name: 'ChooseShop',
  data(){
    return {

    }
  },
  methods: {
    backTo() {
      this.$router.go(-1);
    }
  },
  components: {
  	NavBar,
    Cards
  }
}
</script>

<style scoped>
	.chos-nav span{
    display: inline-block;
    font-size: 20px;
    margin-left: 10px;
    margin-right: 5px;
  }
  .chos-nav p {
    display: inline-block;
  }

  .cards-item {
    width: 100%;
  }

  #myTab li {
    width: 50%;
  }
  #myTab a {
    text-align: center;
  }
  .chooseActive {
    color: #ffb872;
  }

  a:link {
    color: grey;
  }


</style>
