<script>
export default{
    data(){
        return{

            links:[
                {
                    image: "img/buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    image: "img/buy-comics-merchandise.png",
                    text: "dc merchandise"
                },
                {
                    image: "img/buy-comics-subscriptions.png",
                    text: "subscription"
                },
                {
                    image: "img/buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    image: "img/buy-dc-power-visa.svg",
                    text: "dc power visa"
                },
            ]
        }
    }
}
</script>

<template>
    
    <section class="shop-section">
        <div class="container-centered">
            
            <div class="links-container">
                <a v-for="link in links" href="#" class="link">
                    <div class="img-container">
                        <img :src="link.image" alt="">
                    </div>
                    <div class="text">
                        {{ link.text.toUpperCase() }}
                    </div>
                </a>

            </div>
           
        </div>
    </section>

</template>

<style scoped lang="scss">

.shop-section{
    display: flex;
    flex-direction: row;
    align-items: center;

    height: 140px;

    background-color: #0282f9;
    .links-container{

        display: flex;
        flex-direction: row;
        justify-content: space-around;
        
        .link{
            display: flex;
            flex-direction: row;
            gap: 10px;

            .img-container{
                height: 50px;
                max-width: 50px;

                img{
                    height: 100%;
                    width: 100%;
                }
            }
            .text{
                display: flex;
                align-items: center;

                font-size: 0.8em;
                color: white;
            }
        }
    }
}
</style>