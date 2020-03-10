<template>
  <div class="hello">
    <swiper></swiper>
    <news></news>
    <Homebutton></Homebutton>
  </div>
</template>

<script>
import swiper from './TopPic/pic'
import news from './midNews/news'
import Homebutton from './BottomButton/InButton'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    swiper,
    news,
    Homebutton 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
