<template>
    <div id="container">
        <Card-Item class="_card" v-for="(article, index) in articles" :key="index"
        :title="article.title"
        :image="article.image"
        :summary="article.summary"
        :date="article.date"
        @onCardSelected="cardSelected"
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
      isCardSelected: false
    }
  },
  methods: {
    cardSelected (selected) {
      this.isCardSelected = selected
      this.$emit('onCardSelected', this.isCardSelected)
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
