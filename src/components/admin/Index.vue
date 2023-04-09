<template>
  <div>
    <NavBar></NavBar>
  	<IndexSwipe></IndexSwipe>

  </div>
</template>

<script>
import IndexSwipe from '@/components/admin/common/IndexSwipe'
import NavBar from '@/components/admin/common/NavBar'
export default {
  name: 'Index',
  data() {
    return {


		}
  },
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    }
  },
  components: {
    NavBar,
  	IndexSwipe

  }
}
</script>

<style scoped>


</style>
