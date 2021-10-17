<template>
  <nav class="navbar navbar-expand-lg navbar-warning bg-warning bg-gradient ">
  <div class="container-fluid">
    <!-- <a class="navbar-brand" href="#">Navbar</a> -->

    <router-link class="navbar-brand text-black" to="/">Gif Route</router-link>
    <button class="navbar-toggler bg-dark" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon bg-warning"></span>
    </button>
    <div class="collapse navbar-collapse text-black " id="navbarNav">
      <ul class="navbar-nav text-black">
        <li class="nav-item text-black">
          <!-- <a class="nav-link active" aria-current="page" href="#">Home</a> -->
        <router-link class="nav-link active text-black" aria-current="page" to="/">Home</router-link>
        </li>
        <li class="nav-item ">
          <!-- <a class="nav-link" href="#">Features</a> -->
          <router-link class="nav-link text-black" to="/about">About</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link text-black" to="/gifs">Gifs</router-link>
        </li>
        <li class="nav-item">
          <router-link  class="nav-link text-black" to="/stickers">Stickers</router-link>
        </li>

     
      </ul>
    </div>
  </div>
</nav>
</template>

<script>
export default {

}
</script>

<style>


</style>