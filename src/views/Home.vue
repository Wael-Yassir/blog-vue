<template>
  <div class="home">
    <Card-Item-List :articles="this.articles" style="margin: 0 5px"/>
  </div>
</template>

<script>

import CardItemList from '../components/Card-Item-List.vue'
import db from '@/db.js'

export default {
  name: 'Home',
  components: {
    CardItemList
  },
  data () {
    return {
      articles: db.articles
    }
  },
  methods: {
  }
}
</script>
