<script>
export default{
    data(){
        return{
            message: "--> Content goes here <--",

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
    <main>
        <section class="sec-one">
            <div class="container-centered">
    
                <div id="test"> {{ message }} </div>
                
            </div>  
        </section>

        <section class="sec-two">
            <div class="container-centered">
                
                <ul class="card-container">
                    <li v-for="card in links" class="card">
                        <div class="img-container">
                            <img :src="card.image" alt="">
                        </div>
                        <div class="text">
                            {{ card.text.toUpperCase() }}
                        </div>
                    </li>

                </ul>
               
            </div>
        </section>
    </main>
</template>

<style scoped lang="scss">

main{
    
    .sec-one{
        display: flex;
        flex-direction: row;
        align-items: center;

        min-height: 100px;

        background-color: #1c1c1c;
        .container-centered{
            margin-left: auto;
            margin-right: auto;
            
            width: 70%;
    
            #test{
                font-size: 1.6em;
                font-weight: bold;
    
                color: white;
            }
        } 
    }

    .sec-two{
        display: flex;
        flex-direction: row;
        align-items: center;

        height: 140px;

        background-color: #0282f9;

        .container-centered{
            margin-left: auto;
            margin-right: auto;
            
            width: 70%;

            .card-container{

                display: flex;
                flex-direction: row;
                justify-content: space-around;
                
                .card{
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

    }

}

</style>