<template>
  <div class="container">
    <h1>Hello</h1>

    <NuxtLink to="/about">About Page</NuxtLink>
  </div>
</template>

<script>
export default {
  layout: 'default',
  name: 'IndexPage',
  data () {
    return {
      ads: []
    }
  },

  methods: {
    async getAds () {
      return await this.$axios.get('http://bugachiev.com/api/nb-board')
    }
  },

  async mounted () {
    let ads = await this.getAds()

    console.log(ads)
  }
}
</script>
