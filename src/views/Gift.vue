<template>
<div class="container mt-3 border">
    <h1 class="text-center">Gifs</h1>
    <hr />
    <div class="row">
        <div class="col-12">
            <gif-card :data="gifs" class="m-3  w-75"/>
        </div>
    </div>
</div>
  
</template>

<script>
import GifCard from '../components/GifCard.vue';
export default {
  components: { GifCard },
    data: () => ({
        gifs: {},
    }),
    created() {
        this.getGifs();
    },

    methods:{
         async getGifs(){
            const { data } =  await this.axios.get("api.giphy.com/v1/gifs/random?api_key=u9k70IglGZzmFNn3nU24QWPhgtcWA7pt");
                this.gifs = data.data;
                console.log(this.gifs)
       },

    }


    
};
</script>

