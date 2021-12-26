<template>
  <div class="page page-index">
    <div class="firstscreen">
       <h1 class="text-center text-white"><span class="fv-normal">Недвижимость и работа Вашей мечты</span>
         <br>
         <br/>
         <span class="text-upper">Квартира, Коммерция, Участок и дом на</span>
         <br>
         <span class="firstscreen__title">BUGACHIEV.COM</span>
       </h1>
    </div>
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
    
  }
}
</script>

<style scoped>
  .firstscreen {
    min-height: 649px;
    background: url('/index/firstscreen.png') no-repeat center center / cover;
    width: 100%;
    padding-top: 150px;
  }

  .firstscreen__title {
    font-size: 65px;
  }
</style>