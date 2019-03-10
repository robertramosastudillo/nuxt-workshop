<template lang="html">
    <div class="">
        <h1>Álbums de la página</h1>
        <AlbumCard :album="album" v-for="album in albums"/>
    </div>
</template>

<script>
import axios from 'axios';
import env from '../config/env';
import AlbumCard from '../components/AlbumCard';
export default {
    name: 'IndexPage',
    components:{
        AlbumCard
    },
    data(){
        return{
            albums: []
        }
    },
    created(){
        axios.get(`${env.endpoint}/albums`).then(response=>{
            this.albums = response.data;
        })
    }
}
</script>

<style scoped>

</style>



