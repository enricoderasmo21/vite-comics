<script>
export default{
    data() {
        return{

            footerLists:[
                {
                    title: "dc comics",
                    links: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
                },
                {
                    title: "shop",
                    links: ["Shop DC", "Shop DC Collectibles"]
                },
                {
                    title: "dc",
                    links: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us",]
                },
                {
                    title: "sites",
                    links: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]

                },
            ],

        }
    }
}
</script>

<template>

        <section class="sec-one">
            <div class="container-centered">
                <div class="inner-sec-one">

                    <div class="link-container">
                        <div v-for="list in footerLists">
                            <h3 class="title"> {{ list.title.toUpperCase() }} </h3>
                            <ul class="link-list">
                                <li v-for="link in list.links" class="link">
                                    {{ link }}  
                                </li>
                            </ul>
                        </div>
                    </div>
    
                    <div class="img-container">
                        <img src="/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </section>
    
</template>

<style scoped lang="scss">
.sec-one{
    height: 300px;

    background-image: url(img/footer-bg.jpg);

    .inner-sec-one{
        display: flex;
        flex-direction: row;
        justify-content: space-between;

        .link-container{
            display: flex;
            flex-direction: row;
            gap: 20px;

            padding-top: 20px;

            .link-list{
                display: flex;
                flex-direction: column;
                gap: 4px;
            }

            .title{
                margin-bottom: 10px;
                font-size: 0.9em;

                color: white;
            }

            .link{
                font-size: 0.6em;

                cursor: pointer;

                color: #959595;
            }
        }
    
        .img-container{
            height: 300px;

            overflow: hidden;
    
            img{
                height: 150%;

                transform: translate(0, -18%);
            }
        }
    }
}
</style>