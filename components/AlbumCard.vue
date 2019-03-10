<template lang="html">
    <div class="column is-one-quarter">
        <div class="box">
            <h3>{{album.title}}</h3> 
            <a href="#" class="button is-primary">Ve álbum</a>
        </div>

    </div>
</template>

<script>
export default {
    name: 'AlbumCard',
    props: {
        album: Object
    }
}
</script>

<style scoped>
    .box{
        padding: 1em;
    }
    h3{
        min-height: 5em; 
    }
</style>

