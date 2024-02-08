<template>
    <div id="comic" class="me-3 mb-5">
        <img :src="propsImg" alt="">
        <p class="text-center">{{ propsTitle }}</p>
    </div>
</template>

<script>

    export default{
        name:"DcComics",
        props :{
            propsImg: String,
            propsTitle: String

        }
    }

</script>

<style lang="scss" scoped>
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;            
    }
</style>