<template>
    <div id="container">
        <Card-Item class="_card" v-for="(article) in articles" :key="article.id"
        :id="article.id"
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
  },
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped>
#container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
._card {
    margin: 4px 8px;
}
._card :hover {
  cursor: pointer;
}
</style>
