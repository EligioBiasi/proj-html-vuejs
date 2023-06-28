<template>
    <div class="jumbotron text-white text-center">
        <h1>
            Inspiring Tomorrows Leaders
        </h1>

        <h3 class="mt-2">
            The Futur Belongs To Those Who See Possibilities Today
        </h3>

        <div class="mt-5">
            <button type="button" class="text-uppercase fw-semibold me-3 text-white orange-button">find a course</button>
            <button type="button" class="text-uppercase fw-semibold lightblue-button">apply now</button>
        </div>
    </div>
</template>

<script>
export default {
    name:'Jumbotron',
    data(){
        return {

        }
    },
    components:{
        
    }
    
}
</script>

<style lang="scss" scoped>
    div.jumbotron{
        background-image: url('../assets/images/home_main_slider_bg.jpg');
        background-position: center;
        padding: 240px 0;
    }

    h1{
        font-size: 4rem;
    }

    button{
        border: none;
        font-size: .8rem;
        padding: .5rem 1rem;
    }

    button.orange-button{
        background-color: #f09a3e;
    }

    button.lightblue-button{
        background-color: #00bcd4;
        color: white;
        
    }

    button.orange-button:hover{
        background-color: #00bcd4;
        transition: all 0.5s;
    }

    button.lightblue-button:hover{
        background-color: white;
        color: black;
        transition: all 0.5s;
    }
</style>