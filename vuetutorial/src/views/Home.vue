<template>
  <v-content>
    <Carousel/>
    <Gallery/>
    <LatestPost/>
  </v-content>
</template>

<script>
import Carousel from '../components/Carousel';
import Gallery from '../components/Gallery';
import LatestPost from '../components/LatestPost';
export default {
  name: 'Home',

  components: {
    Carousel,
    Gallery,
    LatestPost,
  },

  data () {
    return {
      items: [
      ]
    }
  },
}
</script>
