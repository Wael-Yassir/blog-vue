<template>
    <div id="container">
        <Card-Item @click.native="show" class="_card" v-for="(article, index) in articles" :key="index"
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
  methods: {
    show: function () {
      console.log('Hello, from card-item!')
    }
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
