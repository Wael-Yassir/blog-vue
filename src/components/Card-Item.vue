<template>
  <div>
    <router-link :to="{
      path: '/article/' + this.id,
    }"
    style="all:unset;">
      <b-card
        :title="title"
        :img-src="image"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 20rem"
        class="mb-2">
        <b-card-text> {{ this.summary }} </b-card-text>
        <div id='date-container'>
          <b-icon icon="calendar3"/>
          <p id="article-date">{{ this.date }}</p>
        </div>
      </b-card>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'Card-Item',
  props: {
    id: Number,
    title: String,
    image: String,
    summary: String,
    date: String
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
  #date-container {
    display: inline;
  }

  #article-date {
    display: inline;
    padding-left: 8px;
  }

  img {
    width: 320px;
    height: 200px;
  }
</style>
