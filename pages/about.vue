<template>
  <div>
    <Navbar/>
    <!-- About Content -->
    <div class="image">
  <b-card no-body class="overflow-hidden" style="max-width: 540px;">
    <b-row no-gutters>
      <b-col md="6">
        <b-card-img src="../assets/image.jpeg" alt="Image" class="rounded-0"></b-card-img>
      </b-col>
      <b-col md="6">
        <b-card-body title="Raka Abdi Rmp">
          <b-card-text>
            Junior Front End Development, Even If It's Not As Great As You Think, But I'm Still Enthusiastic
            <br><br> Berhenti Menyalahkan Segalanya -17th
          </b-card-text>
        </b-card-body>
      </b-col>
    </b-row>
  </b-card>
</div>
  </div>
</template>

<script>
export default {
  name: 'about'
}
</script>

<style>
.image {
  margin-left: 380px;
  margin-top: 140px;
}
</style>
