<script>
  import DcHeader from './components/DcHeader.vue'
  import DcMain from './components/DcMain.vue'

  export default{
    components: {
      DcHeader,
      DcMain,
    }
  }
  
</script>

<template>

  <DcHeader/>
  <DcMain/>
</template>

<style lang="scss">
  @use './styles/general.scss'
</style>
