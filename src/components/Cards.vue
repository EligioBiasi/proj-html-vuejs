<template>
    <div class="d-flex">
        <div class="card-section position-relative" v-for="img in imgList">
            <img :src="getImagePath(img)" alt="" class="d-block">

            <div class="position-absolute top-50 start-50 translate-middle text-white text-center">
                <h2>
                    {{ img.toUpperCase() }}
                </h2>
                <div class="line mt-3"></div>
                <p class="mt-3">
                    View More
                </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Cards',
    data(){
        return {
            imgList:['courses','events','latest news'],
        }
    },
    components:{
        
    },

    methods: {
        getImagePath(img){
        return new URL(`../assets/images/home_${img}_section_bg.jpg`, import.meta.url).href;
      },
    },
    
}
</script>

<style lang="scss" scoped>
    div.card-section {
        position: relative;
        width: calc(100% / 3);
        overflow: hidden;
        }
    div.line{
        width: 50px;
        background-color: goldenrod;
        height: 1px;
        margin: 0 auto;
    }

    img {
        width: 100%;
        transition: transform 2s ease;
        }

    div.card-section:hover img {
        transform: scale(1.2);
        filter: brightness(1.5);
        }
</style>