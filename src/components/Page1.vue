<template>
    <div>
        Refresh current page, you'll see a different Skeleton!
        <router-link to="/">Jump to Home{{a}}</router-link>
    </div>
</template>

<script>
export default {
    name: 'page1',
    data(){
      return{
        a:""
      }
    },
    mounted() {
      this.a = this.$route.params.type
    },
};
</script>
