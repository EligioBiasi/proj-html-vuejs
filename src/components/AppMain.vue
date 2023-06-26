<template>
    <main>
        <Jumbotron />
        <central />
        <Values />
    </main>
</template>

<script>
import central from "./central.vue";
import Jumbotron from "./Jumbotron.vue";
import Values from "./Values.vue";

export default {
    name:'AppMain',
    data(){
        return {

        }
    },
    components:{
        Jumbotron,
        central,
        Values,
    }
    
}
</script>

<style lang="scss" scoped>
    
</style>