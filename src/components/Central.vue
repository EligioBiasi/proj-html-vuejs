<template>
    <div class="container my-5">
        <div class="text-center mb-5">
            <img src="../assets/images/page-logo-1.png" alt="">
            <h3 class="mt-3">Inspired By Excellence & Innovation</h3>
            <p class="mt-4">We offer a wide range of high quality of theaching and extra-curricular activities</p>
            <div class="line"></div>
        </div>

        <div class="d-flex">
            <div class="col-7">
                <h5 class="text-uppercase mb-3">
                    why choose avada university
                </h5>
                <p class="lh-lg">
                    We offer a range of training packages in a range of subject areas and can offer blended learning opportunities to best meet your needs. if sitting in a room with a trainer and having the opportunity for discussion with other learners sounds good to you then we can offer this. If you prefer to study in your own time and at your own speed than one of our world class facilities.
                </p>
                <p class="lh-lg">
                    If you prefer to study in your own time and at your own speed then one of our e-learning packages may be right up your street. There is a third option, which is you like the sound of both but perhaps can't attend all training session, this is when Harry Potter, the boy who lived, come to die... avada kedavra! 
                </p>
            </div>

            <div class="col-4 ms-auto">
                <video src="../assets/images/Cambridge!.mp4" controls width="100%" height="100%" muted>
                </video>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'central',
    data(){
        return {

        }
    },
    components:{
        
    }
    
}
</script>
<style lang="scss" scoped>
    

    h3{
        color: #333c4e;
    }

    p{
        color: #7e8890;
        font-size: .9rem;
    }

    div.line{
        width: 200px;
        background-color: goldenrod;
        margin: 0 auto;
        height: 1px;
    }
</style>