<template>
    <footer>
        <Form />
        <information />
        <bottomFooter />
    </footer>
</template>

<script>
import Form from "./Form.vue";
import information from "./Information.vue";
import bottomFooter from "./BottomFooter.vue";

export default {
    name:'AppFooter',
    data(){
        return {

        }
    },
    components:{
        Form,
        information,
        bottomFooter,
    }
    
}
</script>

<style lang="scss" scoped>
    
</style>