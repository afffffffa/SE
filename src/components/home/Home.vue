<template>
  <div>
    <NavBar style="font-family: Arial, sans-serif; background-color: #f5f5f5; color: #333;">
      <div slot="nav-text"><p style="font-weight: bold; font-size: 20px;">南方科技大学食堂</p></div>
    </NavBar>

    <Swipe></Swipe>
    <Options></Options>
    <TabBar></TabBar>
  </div>
</template>

<script>
import NavBar from '@/components/common/NavBar'
import Swipe from '@/components/home/Swipe'
import Options from '@/components/home/Options'
import TabBar from '@/components/tabbar/TabBar'
export default {
  name: 'Home',
  components: {
  	NavBar,
    Swipe,
    Options,
    TabBar
  }
}
</script>

<style>

</style>
