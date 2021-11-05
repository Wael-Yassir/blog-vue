<template>
  <div class="home">
    <Card-Item-List :articles="this.articles" style="margin: 0 5px" class=""/>
  </div>
</template>

<script>

import CardItemList from '../components/Card-Item-List.vue'

export default {
  name: 'Home',
  components: {
    CardItemList
  },
  data () {
    return {
      articles: [
        {
          title: 'title1',
          image: 'https://wallpaperaccess.com/full/176937.jpg',
          summary: "Some quick example text to build on the card title and make up the bulk of the card's content.",
          date: '10.10.2021'
        },
        {
          title: 'title2',
          image: 'https://wallpaperaccess.com/full/12919.jpg',
          summary: "Some quick example text to build on the card title and make up the bulk of the card's content.",
          date: '15.09.2021'
        },
        {
          title: 'title4',
          image: 'https://i.pinimg.com/originals/86/ff/b8/86ffb87572d657f335cd7cd828c70de3.jpg',
          summary: "Some quick example text to build on the card title and make up the bulk of the card's content.",
          date: '05.03.2021'
        },
        {
          title: 'title3',
          image: 'https://www.pixel4k.com/wp-content/uploads/2019/06/reindeer-digital-art-4k_1560535395.jpg',
          summary: "Some quick example text to build on the card title and make up the bulk of the card's content.",
          date: '07.04.2021'
        }
      ]
    }
  }
}
</script>
