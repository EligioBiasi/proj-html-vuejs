<template>
    <hr>
    <div class="d-flex justify-content-between px-5 py-1">
        <div>
            <ul class="d-flex">
                <li v-for="right in rightsList">
                    {{ right }}
                </li>
            </ul>
        </div>

        <div>
            <i class="fa-brands fa-facebook-f" style="color: #7e8890;"></i>
            <i class="fa-brands fa-twitter" style="color: #7e8890;"></i>
            <i class="fa-brands fa-youtube" style="color: #7e8890;"></i>
            <i class="fa-brands fa-instagram" style="color: #7e8890;"></i>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            rightsList:['Theme Fusion','All Rights Reserved','Powered by WordPress', 'support@fusion.com', '1.800.555.6789']
        }
    },

}
</script>

<style lang="scss" scoped>
    ul{
        list-style-type: none;
    }

    li{
        font-size: 0.5rem;
        color: #7e8890;
        padding: 0 .5rem;
        border-right: solid 1px #7e8890;
    }

    i{
        padding-left: 1rem;
    }
</style>