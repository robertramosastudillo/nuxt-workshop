<template lang="html">
    <h1>Hola mundo</h1>  
</template>

<script>
import router from 'vue-router';
export default {
    name: 'AlbumIndvPage',
    created(){
        let albumId = this.$route.params.id;
        console.log(albumId);
    }
}
</script>

<style scoped>

</style>
