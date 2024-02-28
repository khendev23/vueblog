<template>
  
  <div>
    <h3>상세페이지</h3>
    <h4>{{posts[$route.params.id].title}}</h4>
    <p>{{posts[$route.params.id].content}}</p>
  </div>
</template>

<script>
export default {
  name : "postDetail",
  props : {
    posts : Array
  }
}
</script>

<style>

</style>