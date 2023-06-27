<template>
    <div class="image-background">
        <div class="d-flex justify-content-around p-5">
            <div>
                <div>
                    <h4 class="text-uppercase">
                        avada univeristy
                    </h4>
                    <ul>
                        <li class="d-flex">
                            <span class="pe-3">
                                <i class="fa-sharp fa-solid fa-house-chimney fa-2xs" style="color: #7e8890;"></i>
                            </span>
                            <div>
                                <span> Residential Location</span>
                                <p>9521 Broadsberry Avenue</p>
                                <p> Paddington RC7 9ZA</p>
                            </div>
                        </li>

                        <li>
                            <i class="fa-solid fa-phone fa-2xs pe-3" style="color: #7e8890;"></i>
                            <span>1.800.458.556</span>
                        </li>

                        <li>
                            <i class="fa-regular fa-envelope fa-2xs pe-3" style="color: #7e8890;"></i>
                            <span>info@your-domain.com</span>
                        </li>

                        <li>
                            <i class="fa-regular fa-clock fa-2xs pe-3" style="color: #7e8890;"></i>
                            <span>Monday - Friday: 8:00 AM - 10:00 PM</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div>
                <h4 class="text-uppercase">
                    recent post
                </h4>

                <ul>
                    <li class="d-flex">
                        <span class="pe-2">
                            <i class="fa-solid fa-angle-right fa-xs" style="color: #a1a1a1;"></i>
                        </span>
                        <div>
                            <a href=""> What do successful grads think you should study</a>
                            <p>
                                March 16, 2016
                            </p>
                        </div>
                    </li>

                    <li class="d-flex">
                        <span  class="pe-2">
                            <i class="fa-solid fa-angle-right fa-xs" style="color: #a1a1a1;"></i>
                        </span>
                        <div>
                            <a href="">Former student discusses success in the fashion industry</a>
                            <p>
                                March 16, 2016
                            </p>
                        </div>
                    </li>

                    <li class="d-flex">
                        <span  class="pe-2">
                            <i class="fa-solid fa-angle-right fa-xs" style="color: #a1a1a1;"></i>
                        </span>
                        <div>
                            <a href="">How do you best prepare for university</a>
                            <p>
                                March 15, 2016
                            </p>
                        </div>
                    </li>
                </ul>
            </div>
        

            <div>
                <div>
                    <h4 class="text-uppercase">
                        Courses
                    </h4>
        
                    <ul>
                        <li>
                            Arts & Humanities
                        </li>
        
                        <li>
                            Business & Managment
                        </li>
        
        
                        <li>
                            Engineering & Technology
                        </li>
        
                        <li>
                            Life Sciences & Medicine
                        </li>
        
                        <li>
                            Natural Sciences
                        </li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-uppercase">
                        Admissions
                    </h4>
        
                    <ul>
                        <li>
                            Eligibility
                        </li>
        
                        <li>
                            Application
                        </li>
        
        
                        <li>
                            Review Process
                        </li>
        
                        <li>
                            How to Apply
                        </li>
                    </ul>
                </div>


            </div>

            <div>
                <div>
                    <h4 class="text-uppercase">
                        resources
                    </h4>
        
                    <ul>
                        <li>
                            Campus Directory
                        </li>
        
                        <li>
                            Academic Calendar
                        </li>
        
        
                        <li>
                            Sports Clubs
                        </li>
        
                        <li>
                            Graduate Programs
                        </li>
        
                        <li>
                            Faculty & Staff
                        </li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-uppercase">
                        quicklinks
                    </h4>
        
                    <ul>
                        <li>
                            University Library
                        </li>
        
                        <li>
                            Campus Services
                        </li>
        
        
                        <li>
                            Careers
                        </li>
                    </ul>
                </div>

            </div>

            <div>
                <h4 class="text-uppercase">
                    upcoming events
                </h4>

                <div v-for=" item in imgLlist" class="mb-4">
                    <div class="d-flex">
                        <img :src="getImagePath(item.img)" alt="" class="pe-2">

                        <div>
                            <p>
                                {{item.date}}
                            </p>
                            <h5 class="fw-bold">
                                {{ item.img }}
                            </h5>
                        </div>
                    </div>
                    <hr>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name:'information',
    data(){
        return {
            imgLlist:[
            {
                img:'politics seminar',
                date: 'November 6 @ 8:00 am'
            },
            {
                img:'business seminar',
                date: 'july 1 @ 8:00 am'
            },
            {
                img:'english seminar',
                date: 'October 17 @ 8:00 am'
            },
        ]
        }
    },
    components:{
      
    },

    methods:{
        getImagePath(img){
        return new URL(`../assets/images/${img}_event_feat-800x536.jpg`, import.meta.url).href;
      },
    }
}
</script>

<style lang="scss" scoped>
    div.image-background{
        background-image: url('../assets/images/university_ft_bg.png');
        object-fit: cover;
    }

    ul{
        list-style-type: none;
        padding: 0;
    }

    p{
        margin: 0;
    }

    li{
        padding-top: .7rem;
    }

    a{
        text-decoration: none;
        font-weight: 600;
        color: #333c4e;
    }

    img{
        width: 110px;
    }

    h4,h5{
        color: #f09a3e;
    }
</style>