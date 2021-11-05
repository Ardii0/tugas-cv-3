<template>
  <div id="app">
    <div class="container">
    <div class="row py-4">
      <cv-satu/>
    </div>
    <br><br>
    <div>
      <cv-dua/>
    </div>
    </div>
  </div>
</template>
<script>
  import CvSatu from './components/CvSatu.vue'
  import CvDua from './components/CvDua.vue'

export default {
  name: 'app',
  components: {
    CvSatu,
    CvDua
  }
}
</script>