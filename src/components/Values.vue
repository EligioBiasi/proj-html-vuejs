<template>
    <div class="lightgray-background">
        <div class="container">
            <div class="d-flex row">

                <div class="col-6">
                    <h3 class="text-uppercase">
                        world class facilities
                    </h3>

                    <p>
                        Avada University is devoted to excellence in teaching learning, and research, and developing leaders in mnay disciplines who make a difference globally.
                    </p>

                    <div class="mb-1">
                        <i class="fa-solid fa-globe fa-lg pe-3" style="color: #f09a3e;"></i>
                        <span class="fw-bold">Internal focus</span>
                        <span class="grey-text"> - our students come from across the globe</span>
                    </div>

                    <div class="mb-1">
                        <i class="fa-solid fa-graduation-cap pe-3" style="color: #f09a3e;"></i>
                        <span class="fw-bold">Internal focus</span>
                        <span class="grey-text"> - our students come from across the globe</span>
                    </div>

                    <div class="mb-1">
                        <i class="fa-solid fa-address-book fa-lg pe-3" style="color: #f09a3e;"></i>
                        <span class="fw-bold">Internal focus</span>
                        <span class="grey-text"> - our students come from across the globe</span>
                    </div>

                    <p>
                        if you prefer to study in your own time and at your own speed then one of our e-learning packages may be right up your street.
                    </p>
                </div>

                <div class="col-6">
                    <h3 class="text-uppercase">
                        our Values
                    </h3>
                    <div>
                            <div class="p-2 d-flex align-items-center">
                            <i class="fa-solid fa-plus fa-lg" style="color: #f09a3e;" data-bs-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample"></i>
                            <span class="text-uppercase fw-bold ms-3 fs-4">
                                our mission
                            </span>
                    </div>
                    <div class="collapse" id="collapseExample">
                                <span class="card card-body">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus pariatur dignissimos aspernatur quasi officia recusandae quae consectetur minus, eum saepe quisquam ipsum, asperiores quia consequatur necessitatibus eaque nam praesentium quas!
                                </span>
                        </div>
                    </div>
                   
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Values',
    data(){
        return {

        }
    },
    components:{
        
    }
    
}
</script>

<style lang="scss" scoped>

    div.lightgray-background{
        background-color: #f7f5f4;
    }

    h3{
        color: #333c4e;
        margin: 0;
    }

    p{
        margin-top: 2rem;
    }

    p,
    span.grey-text{
        color: #7e8890;
    }
</style>