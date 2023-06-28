<template>
    <div class="bg-white w-100">
        <div class="container d-flex align-items-center py-4">
            <div>
                <img src="..//assets/images/university-logo-retina.png" alt="logo university" class="w-50">
            </div>

            <nav class="ms-auto">
                <ul class="d-flex">
                    <li v-for="navItem in navList" class="mx-4">
                        {{navItem.toUpperCase()}}
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>

export default {
    name:'BottomHeader',
    data(){
        return {
            navList:['home','about','courses', 'events', 'facilities', 'news', 'admissions'],
        }
    },
    components:{
        
    }
    
}
</script>

<style lang="scss" scoped>
    ul{
        list-style-type: none;
        li{
            font-weight: bold;
            font-size: .9rem;
        }
    }
</style>