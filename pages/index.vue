<template>
  <main>
    <Navbar/>
  <b-container fluid="xl" class="text-1">
    <h2>Quoates Anjay</h2>
    <p>Read, Think, Inspiration, You Can Do It</p>
  </b-container>
  <img src="../assets/book.gif" id="image-profil" width="200px">
  </main>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>
body {
  margin: 0;
}
.text-1 {
  position: absolute;
  top: 300px;
  left: 200px;
}
#image-profil {
  position: absolute;
  left: 800px;
  top: 230px;
}
h2 {
  font-weight: bold;
  color: rgb(91, 91, 255);
}
</style>
