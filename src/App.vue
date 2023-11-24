<template>
  <img alt="Vue logo" src="./assets/logo.png">
  
  <div class="menu">
    <a>HOME</a>
    <a>Products</a>
    <a>About</a>
  </div>
  
  <div>
    <h4 :style="colorBlue">{{ products[0] }}</h4>
    <p>{{ price1 }} 만원</p>
  </div>
  <div>
    <h4 :style="colorBlue">{{ products[1] }}</h4>
    <p>{{ price2 }}</p>
  </div>
  <div>
    <h4 :style="colorBlue">{{ products[2] }}</h4>
    <p>{{ price2 }}</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      products : ['역삼동원룸', '천호동원룸', '마포구원룸'],
      price1 : 50,
      price2 : "가격은 아무거나",
      colorBlue : {
        color : 'blue'
      }
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding: 10px;
}
</style>
