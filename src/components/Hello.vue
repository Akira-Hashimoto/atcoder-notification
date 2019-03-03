<template>
  <div class="hello">
    <input type="text" name="namae" size="40" maxlength="20" v-model="ref">
    <br>
      <li><a v-bind:href="'https://atcoder.jp/users/' + ref" target="_blank" rel="noopener">{{search}}</a></li>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      ref: 'User Name',
      search: 'Userを検索する'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
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
  color: #35495E;
}
</style>
