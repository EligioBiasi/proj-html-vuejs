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
                    <li class="d-flex" v-for="item in postList">
                        <span class="pe-2">
                            <i class="fa-solid fa-angle-right fa-xs" style="color: #a1a1a1;"></i>
                        </span>
                        <div>
                            <a href="" class="question">{{item.question}}</a>
                            <p>
                                {{ item.date }}
                            </p>
                        </div>
                    </li>
                </ul>
            </div>
        

            <div>
                <div v-for="item in itemsLists">
                    <h4 class="text-uppercase">
                        {{item.title}}
                    </h4>
        
                    <ul>
                        <li v-for="voice in item.voices">
                            <a href="" class="text-black">{{voice}}</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div>
                <div v-for="item in itemsList2">
                    <h4 class="text-uppercase">
                        {{item.title}}
                    </h4>
        
                    <ul>
                        <li  v-for="voice in item.voices">
                            <a href="" class="text-black">{{voice}}</a>
                           
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
            postList:[{
                question:'What do successful grads think you should study',
                date:'March 16, 2016'
            },
            {
                question:'Former student discusses success in the fashion industry',
                date:'March 15, 2016'
            },
            {
                question:'How do you best prepare for university',
                date:'March 15, 2016'
            },

            ],

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
        ],
            itemsLists:[
                {
                   title:'Courses',
                   voices:['Business & Managment','Engineering & Technology','Life Sciences & Medicine','Natural Sciences']
                },
                {
                   title:'admissions',
                   voices:['Eligibility','Application','Review Process','How to Apply']
                },
                
            ],
            itemsList2:[
                {
                   title:'resources',
                   voices:['Campus Directory','Academic Calendar','Sports Clubs','Graduate Programs','Faculty & Staff']
                },
                {
                   title:'quicklinks',
                   voices:['University Library','Campus Services','Careers']
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
    }
    a.question{
        font-weight: 600;
        color: #333c4e;
    }

    a.text-black{
        color: black;
    }

    img{
        width: 110px;
    }

    h4,h5{
        color: #f09a3e;
    }
</style>