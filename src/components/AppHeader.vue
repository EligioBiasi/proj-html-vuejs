<template>
    <header>
        <TopHeader />
        <BottomHeader />
    </header>
</template>

<script>
import TopHeader from "./TopHeader.vue";
import BottomHeader from "./BottomHeader.vue";

export default {
    name:'AppHeader',
    data(){
        return {

        }
    },
    components:{
        TopHeader,
        BottomHeader,
    }
    
}
</script>

<style lang="scss" scoped>
    
</style>