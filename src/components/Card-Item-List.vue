<template>
    <div id="container">
        <Card-Item class="_card" v-for="(article, index) in articles" :key="index"
        :title="article.title"
        :image="article.image"
        :summary="article.summary"
        :date="article.date"
        />
    </div>
</template>

<script>

import CardItem from '../components/Card-Item.vue'

export default {
  name: 'Card-Item-List',
  props: ['articles'],
  components: {
    CardItem
  }
}
</script>

<style scoped>
#container {
    display: flex;
    flex-wrap: wrap;
}
._card {
    margin: 4px 8px;
}
</style>
