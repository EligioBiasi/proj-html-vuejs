<template>
    <div class="orange-background">
        <div class="container py-3 d-flex">
            <div class="text-white d-flex align-items-center">
                <i class="fa-solid fa-phone fa-2xs" style="color: #ffffff;"></i>
                <span class="d-flex align-items-center">1.800.567.8910
                    <span class="gray-pill">24 hrs</span>
                </span>
                <i class="fa-solid fa-envelope fa-xs" style="color: #ffffff;"></i>
                <span>Contact us</span>
                <i class="fa-solid fa-graduation-cap fa-xs" style="color: #ffffff;"></i>
                <span>Alumni</span>
                <i class="fa-solid fa-landmark fa-xs" style="color: #ffffff;"></i>
                <span>Campus</span>
            </div>

            <div class="text-white d-flex align-items-center ms-auto">
                <i class="fa-brands fa-facebook-f" style="color: #ffffff;"></i>
                <i class="fa-brands fa-twitter" style="color: #ffffff;"></i>
                <i class="fa-brands fa-youtube" style="color: #ffffff;"></i>
                <i class="fa-brands fa-instagram" style="color: #ffffff;"></i>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name:'TopHeader',
    data(){
        return {

        }
    },
    components:{
        
    }
    
}
</script>

<style lang="scss" scoped>
    div.orange-background{
        background-color: #f09a3e;

        i{
            margin: 0 1rem;
        }
    }

    span.gray-pill{
        padding: 0 .2rem;
        background-color: lightgray;
        font-size: .5rem;
        border-radius: 12%;
        margin-left: .3rem;
    }

</style>