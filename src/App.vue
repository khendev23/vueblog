<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">Vuelog</router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link active" aria-current="page" href="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/list" class="nav-link" href="#">List</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="mt-4">
    <router-view :posts="posts"></router-view>
  </div>

  <!-- <List :posts="posts"/> -->

</template>

<script>
// import List from './components/List.vue'
import post from './assets/Post'

export default {
  name: 'App',
  data() {
    return {
      posts : post
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

}
</style>
