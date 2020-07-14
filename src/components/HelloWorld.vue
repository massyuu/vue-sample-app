<template>
  <div class="hello">
    <h1>{{ h1_title }}</h1>
    <input v-model="message" placeholder="メッセージをどうぞ">
    <p>入力されたメッセージは「 {{ message }} 」です</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    h1_title: String
  },
  data () {
    return {
      message: ''
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
