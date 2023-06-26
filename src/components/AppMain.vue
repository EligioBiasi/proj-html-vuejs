<template>
    <main>
        <Jumbotron />
        <central/>
    </main>
</template>

<script>
import central from "./central.vue";
import Jumbotron from "./Jumbotron.vue";

export default {
    name:'AppMain',
    data(){
        return {

        }
    },
    components:{
        Jumbotron,
        central,
    }
    
}
</script>

<style lang="scss" scoped>
    
</style>