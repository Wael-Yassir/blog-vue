<template>
  <div>
    <h1>{{ article.title }}</h1>
    <div class="article-img">
      <img :src="article.image" alt="img">
    </div>
    <div style="text-align:left; margin: 0 10px;">
      <h3 >{{ article.summary }}</h3>
      <div class="article-body">
        <h5 style="margin-top: 5px;">{{ article.body }}</h5>
      </div>
    </div>
  </div>
</template>

<script>
import db from '@/db.js'
export default {
  data () {
    return {
      id: this.$route.params.id
    }
  },
  computed: {
    article () {
      return db.articles.find(
        article => article.id === Number(this.id)
      )
    }
  }
}
</script>

<style>
  .article-img {
    margin: 10px;
  }
  .article-img img {
    width: 100%;
    height: auto;
  }
</style>>
