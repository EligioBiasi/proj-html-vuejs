<template>
    <main>
        <Jumbotron />
        <central />
        <Values />
        <Cards />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import central from "./central.vue";
import Values from "./Values.vue";
import Cards from "./Cards.vue";

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
        Cards,
    }
    
}
</script>

<style lang="scss" scoped>
    
</style>