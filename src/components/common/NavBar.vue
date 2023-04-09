<template>

  <div class="navbar">
    <div><slot name="back-to"></slot></div>
    <div><slot name="nav-text"></slot></div>
  </div>
</template>


<script>

export default {
  name: 'NavBar'
}

</script>
@import url('https://fonts.googleapis.com/css?family=Roboto');
<style>
	.navbar {
    height: 80px;
    box-shadow: 0px 1px 1px rgba(100,100,100,0.1);
  }


  .navbar p {
    margin-top: 10px;
    margin-left: 10px;
    color: #000;
    /*font-family: 'Roboto', sans-serif;*/
    font-size: 30px;
    font-weight: bold;
    font-family: "Segoe Script", cursive;
  }
  @keyframes blink {
    50% {
      text-shadow: none;
    }
  }

  @keyframes blink {
    50% {
      text-shadow: none;
    }
  }
  .navbar span {
    display: inline-block;
    margin-left: 5px;
  }
  .chos-nav span{
    display: inline-block;
    font-size: 20px;
    margin-left: 10px;
    margin-right: 5px;
  }
  .chos-nav p {
    display: inline-block;
  }
</style>
