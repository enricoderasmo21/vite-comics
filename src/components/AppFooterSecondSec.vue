<script>
export default{
    data() {
        return{

            socialIconsList: ["img/footer-facebook.png", "img/footer-periscope.png", "img/footer-pinterest.png", "img/footer-twitter.png", "img/footer-youtube.png",]
        }
    }
}
</script>

<template>

        <section class="sec-two">
            <div class="container-centered">
                <div class="sec-two-inner">

                    <button id="sign-btn">SIGN-UP NOW!</button>
                    
                    <div class="inner-right">
                        <div class="follow-us">
                            FOLLOW US
                        </div>
                        <div class="icons-container">
                            <div v-for="icon in socialIconsList" class="img-container">
                                <img :src="icon" alt="">
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </section>
    
</template>

<style scoped lang="scss">
.sec-two{
    display: flex;
    align-items: center;

    height: 100px;

    background-color: #303030;

    .sec-two-inner{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;

        height: 100px;

        #sign-btn{
            padding: 10px;

            background: none;

            border: 2px solid #0282f9;

            color: white;

            cursor: pointer;
        }

        .inner-right{
            display: flex;
            flex-direction: row;

            .follow-us{
                padding-right: 30px;
                
                font-weight: bold;

                color: #0282f9;
            }

            .icons-container{
                display: flex;
                flex-direction: row;
                align-items: center;
                gap: 16px;


                .img-container{
    
                    width: 32px;
    
                    img{
                        width: 100%;

                        cursor: pointer;
                    }
                }
            }

        }

    }

}
</style>