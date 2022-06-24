<template>
  <div class="home">
    <headers/>
    <welcome/>
    <features/>
    <download/>
    <contact/>
    <footers/>
  </div>
</template>

<script>
import headers from '../components/headers.vue'
import welcome from '../components/welcome.vue'
import features from '../components/features.vue'
import download from '../components/download.vue'
import contact from '../components/contact.vue'
import footers from '../components/footers.vue'
export default {
  name: 'Home',
  components: { headers, welcome, features, download, contact, footers },
  mounted() {
    document.title = "3D Software"
  }
}
</script>
