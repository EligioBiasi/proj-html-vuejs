<template>
    <div class="blue-background py-5">
        <div class="container text-center">
            <div class="position-relative">
                <h3 class="text-white">
                    Joining Over <span class="number">500,000 Students</span> Enjoying Avada Education now
                </h3>
                 <svg xmlns="http://www.w3.org/2000/svg" width="250" height="130" viewBox="0 0 120 120" class="position-absolute">
                    <path d="M0,100 Q150,60 220,120" fill="none" stroke="#f09a3e" stroke-width="4" />
                </svg> 
            </div>
            <p class="mb-5">
                Become Part of Avada University To Further Your Career.
            </p>

            <div  class="d-flex justify-content-center">
                <input type="mail" v-for="item in FormItems" :placeholder="item" class="me-2 border-0 py-1 ps-2 saturated">
                <button class="text-uppercase border-0 fw-semibold text-white orange-button">apply now</button>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    name:'Form',
    data(){
        return {
            FormItems:['Name', 'Email', 'Telephone'],
        }
    },
    components:{
        
    }
    
}
</script>

<style lang="scss" scoped>
    .blue-background{
        background-color: #333c4e;
    }

    span.number{
        color: #f09a3e;
    }

    svg{
        top: -3.7rem;
        right: 52%;
    }

    p{
        color: #7e8990;
    }
    input.saturated {
        background-color: #2c3242;
        width: calc(100% / 4);

    }
    button.orange-button{
        width: calc(100% / 6);
    }
    .orange-button{
        background-color: #f09a3e;
    }
</style>