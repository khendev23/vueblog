<template>
  <div v-for="(post, i) in posts" :key="i">
    <h5 @click="$router.push('/detail/' + post.number)">{{post.title}}</h5>
    <p>{{post.date}}</p>
  </div>
</template>

<script>

export default {
  name : 'postList',
  props : {
    posts : Array
  }
}
</script>

<style>

</style>