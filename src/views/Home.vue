<template>
  <div class="home">
    <headers/>
    <welcome/>
    <features/>
    <download/>
  </div>
</template>

<script>
import headers from '../components/headers.vue'
import welcome from '../components/welcome.vue'
import features from '../components/features.vue'
import download from '../components/download.vue'

export default {
  name: 'Home',
  components: { headers, welcome, features, download },
  mounted() {
    document.title = "3D Software"
  }
}
</script>
