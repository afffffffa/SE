<template>
  <div>
    <div class="navbars">
      <div class="navbar-right">
        <div class="navbar-school-logo">
          <img src="../../../assets/img/logo/logo.png" style="width: 380px">
        </div>
      </div>
      <el-menu
        default-active="2"
        class="el-menu-demo"
        mode="horizontal"
        background-color="transparent"
        text-color="#fff"
        active-text-color="#ff7f50"
        router>
        <el-submenu index="1">
          <template slot="title">
            <i class="el-icon-location"></i>
            <span>店铺管理</span>
          </template>
          <el-menu-item-group>
            <!-- <template slot="title">分组一</template> -->
            <router-link to="/shopinfo">
              <el-menu-item index="1-1">店铺信息</el-menu-item>
            </router-link>
            <router-link to="/salesman">
              <el-menu-item index="1-2">店员信息</el-menu-item>
            </router-link>
            <!-- <router-link to="/shopdiscount">
              <el-menu-item index="1-3">优惠券</el-menu-item>
            </router-link> -->
          </el-menu-item-group>
        </el-submenu>

        <el-submenu index="2">
          <template slot="title">
            <i class="el-icon-s-goods" style="font-size: 20px; margin-right: 10px;"></i>商品管理
          </template>

          <!-- <el-menu-item index="2-1-1">上架商品</el-menu-item>
          <el-menu-item index="2-1-2">下架商品</el-menu-item> -->
          <router-link to="/allgoods">
            <el-menu-item index="2-1">所有商品</el-menu-item>
          </router-link>
          <router-link to="/allgoods">
            <el-menu-item index="2-2">商品分类</el-menu-item>
          </router-link>
          <router-link to="/allgoods">
            <el-menu-item index="2-3">编辑商品</el-menu-item>
          </router-link>

          <!--	        <el-submenu index="2-2">-->
          <!--	          <template slot="title">商品规格管理</template>-->
          <!--	          <router-link to="/extrainfo">-->
          <!--		          <el-menu-item index="2-2-1">商品分类</el-menu-item>-->
          <!--		        </router-link>-->
          <!--		       	<router-link to="/extrainfo">-->
          <!--		          <el-menu-item index="2-2-2">温度档位</el-menu-item>-->
          <!--		        </router-link>-->
          <!--		        <router-link to="/extrainfo">-->
          <!--		          <el-menu-item index="2-2-3">甜度档位</el-menu-item>-->
          <!--		        </router-link>-->
          <!--	        </el-submenu>-->
        </el-submenu>

        <el-submenu index="3">
          <template slot="title">
            <i class="el-icon-s-order" style="font-size: 20px; margin-right: 10px;"></i>订单管理
          </template>
          <router-link to="/allorder">
            <el-menu-item index="3-1">所有订单</el-menu-item>
          </router-link>
          <router-link to="/waitingorder">
            <el-menu-item index="3-2">待处理订单</el-menu-item>
          </router-link>
          <router-link to="/finishorder">
            <el-menu-item index="3-3">已完成订单</el-menu-item>
          </router-link>
        </el-submenu>

        <el-submenu index="4">
          <template slot="title">
            <i class="el-icon-s-data" style="font-size: 20px; margin-right: 10px;"></i>统计分析
          </template>
          <router-link to="/todaysell">
            <el-menu-item index="4-1">销售统计</el-menu-item>
          </router-link>
          <router-link to="/todaysell">
            <el-menu-item index="4-1">商品统计</el-menu-item>
          </router-link>
          <!-- <el-menu-item index="4-2">更多统计</el-menu-item> -->
        </el-submenu>

      </el-menu>

    </div>
  </div>
</template>

<script>

export default {
  name: 'NavBar',
  data(){
  	return {
  		isCollapse: true,
  	}
  },
  components: {

  }
}
</script>

<style scoped>
	/*.navbars {*/
	/*	width: 20%;*/
	/*	background-color: #ffa54d;*/
	/*	height: 900px;*/
  /*}*/
  .navbars {
    background-image: linear-gradient(to right, #ff8c00, #ff7f50);
    font-size: 20px; /* 调整字体大小 */
    height: 80px; /* 调整顶部栏高度 */
    display: flex;
    justify-content: center;
    align-items: center;

    /*text-transform: uppercase; !* 将字母转化为大写 *!*/
    letter-spacing: 5px; /* 调整字母间距 */
    font-weight: bold; /* 加粗字体 */
    /* 其他原有样式 */

  }

  .el-menu-demo {
    /*font-size: 20px; !* 调整字体大小 *!*/
    font-family: 'Roboto', sans-serif!important;
  }

  .el-submenu__title:hover {
    color: #ff7f50!important;
  }
  .el-menu-item {
    color: #ff7f50!important;
  }
  .el-menu-item:hover {
    color: #ff7f50 !important;

  }
  .el-menu-item.is-active {
    color: #ff7f50 !important;
  }

</style>
