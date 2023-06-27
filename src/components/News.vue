<template>
    <div class="lightgray-background py-4">
        <div class="container my-5">
            <div class="text-center mb-5">
                <img src="../assets/images/page-logo-1.png" alt="">
                <h3 class="mt-3">Today's Univeristy News</h3>
                <p class="mt-4">Covering topics classes to politics and student organization events.</p>
                <div class="line"></div>
            </div>
            <div class="d-flex">
                <div class="card" v-for="img in imgList">
                    <img :src="getImagePath(img.imgRef)" class="card-img-top rounded-0" alt="#">
                    <div class="card-body rounded-0">
                        <h5 class="card-title">{{ img.title }}</h5>
                        <p class="card-text">By <span class="admin">admin</span> | March 16th, 2016</p>
                        <div class="d-flex align-items-center">
                            <a href="#" class="">Read More ></a>
                            <i class="fa-regular fa-comments fa-2xs ms-auto" style="color: #f09a3e;"> 0</i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'News',
    data(){
        return {
            imgList:[
                {
                imgRef:'header_1',
                title: 'What do successful grads think you should study?',
            },
            {
                imgRef:'header_2',
                title: 'Former student discusses success in the fashion industry',
            },
            {
                imgRef:'header_3',
                title: 'How do you best prepare for univeristy?',
            },
        ],
        }
    },
    components:{
        
    },

    methods:{
        getImagePath(img){
        return new URL(`../assets/images/news_single_post_${img}-800x444.jpg`, import.meta.url).href;
      },
    }
    
}
</script>

<style lang="scss" scoped>
    div.line{
        width: 150px;
        background-color: goldenrod;
        height: 1px;
        margin: 0 auto;
    }

    div.card{
        width: calc(100/3);
        margin-right: 2rem;
        border: none;
    }

    div.lightgray-background{
        background-color: #f7f5f4;
    }

    h5{
        font-size: 1.2rem;
        font-weight: bold;
    }

    h5,
    a,
    span.admin{
        color: #f09a3e;
    }

    a{
        text-decoration: none;
    }

    p,
    a{
        font-size: .7rem;
    }
</style>