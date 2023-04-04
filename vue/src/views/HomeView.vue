<template>
  <div class="home">
    <Card
      v-for="tvshow in tvshows"
      :key="tvshow.name"
      :title="tvshow.name"
      :streaming="tvshow.streaming"
      :image="tvshow.image"
    />
  </div>
</template>

<script>
import Card from '../components/Card.vue'
import { store } from '../components/store'
export default {
  name: 'Home',
  components: {
    Card
  },
  data() {
    return {
      store,
      tvshows: [
        {
          name: 'Gilmore Girls',
          image: 'https://flxt.tmsimg.com/assets/p184655_b_v10_av.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Friends',
          image:
            'https://i.shgcdn.com/3cfb514f-e69c-4450-8bcc-86f8474e5fb6/-/format/auto/-/preview/3000x3000/-/quality/lighter/',
          streaming: 'HBO Max'
        },
        {
          name: 'The Office',
          image:
            'https://roost.nbcuni.com/bin/viewasset.html/content/dam/Peacock/Campaign/landingpages/library/theoffice/mainpage/office-social-min.png/_jcr_content/renditions/original',
          streaming: 'Peacock'
        },
        {
          name: 'The Vampire Diaries',
          image: 'https://flxt.tmsimg.com/assets/p3563021_b_v8_bb.jpg',
          streaming: 'HBO Max'
        },
        {
          name: 'How I Met Your Mother',
          image: 'https://flxt.tmsimg.com/assets/p185124_b_v9_aj.jpg',
          streaming: 'Hulu'
        },
        {
          name: 'Breaking Bad',
          image:
            'https://m.media-amazon.com/images/M/MV5BN2VjOTkwMjgtYWEyMy00MzNmLTllMjktNDI1ZmRhYTAwYTg1XkEyXkFqcGdeQXVyNjAwNDUxODI@._V1_FMjpg_UX1000_.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Arrested Development',
          image:
            'https://img4.hulu.com/user/v3/artwork/92c225ee-2d39-4cb3-a43b-fbcffbefeeb4?base_image_bucket_name=image_manager&base_image=a73fca41-dc41-4d1d-a515-817375bc8853&size=1200x630&format=jpeg',
          streaming: 'Netflix'
        },
        {
          name: 'Outer Banks',
          image: 'https://staticg.sportskeeda.com/editor/2023/02/b0226-16755208881191-1920.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Ted Lasso',
          image:
            'https://m.media-amazon.com/images/M/MV5BMTdmZjBjZjQtY2JiNS00Y2ZlLTg2NzgtMjUzMGY2OTVmOWJiXkEyXkFqcGdeQXVyMDM2NDM2MQ@@._V1_.jpg',
          streaming: 'Apple TV'
        },
        {
          name: 'Shrinking',
          image:
            'https://m.media-amazon.com/images/M/MV5BYzhjMDIwOTgtYmMwNC00ZDIyLWJiMzUtMDM0YTY3M2VmOWNiXkEyXkFqcGdeQXVyMjkwOTAyMDU@._V1_FMjpg_UX1000_.jpg',
          streaming: 'Apple TV'
        },
        {
          name: 'A Series of Unfortunate Events',
          image:
            'https://m.media-amazon.com/images/M/MV5BMTYzMjA3OTgxOV5BMl5BanBnXkFtZTgwMjAwMDU5NjM@._V1_.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Emily In Paris',
          image:
            'https://m.media-amazon.com/images/M/MV5BYjg0OTY5N2UtZDljZS00NDc2LWI1MDAtMDdmN2Q3OTNkMjA1XkEyXkFqcGdeQXVyMTUzMTg2ODkz._V1_.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Gossip Girl',
          image:
            'https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/91I8ElmqRZL._AC_UF894,1000_QL80_.jpg',
          streaming: 'HBO Max'
        },
        {
          name: 'Stranger Things',
          image:
            'https://m.media-amazon.com/images/M/MV5BMDRjYWI5NTMtZTYzZC00NTg4LWI3NjMtNmI3MTdhMWQ5MGJlXkEyXkFqcGdeQXVyNTg4MDc4Mg@@._V1_.jpg',
          streaming: 'Netflix'
        },
        {
          name: 'Euphoria',
          image: 'https://flxt.tmsimg.com/assets/p16805962_b_h9_aa.jpg',
          streaming: 'HBO Max'
        }
      ]
    }
  },

  methods: {}
}
</script>

<style>
.home {
  display: flex;
  width: 90vw;
  flex-wrap: wrap;
}
</style>
