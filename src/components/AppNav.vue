<script>
export default{
    data(){
        return{
            links:["charachters", "comics", "movies", "tv", "games", "collectibles", "videos", "fans", "news", "shop"],

            activeIndex: 1,
        }
    },

    methods:{

        activeLink(index){
            this.activeIndex = index; 
        }

    }
}
</script>

<template>
    
        <div class="container-centered">
            <nav>

                <div id="logo">
                    <img src="/img/dc-logo.png" alt="dc-logo">
                </div>

                <div>
                    <ul id="links-container">
                        <li v-for="(link, index) in links" @click="activeLink(index)" :class="index == activeIndex ? 'active' : '' " class="link"> {{ link.toUpperCase() }} </li>
                    </ul>
                </div>

            </nav>
        </div>

</template>

<style scoped lang="scss">

nav{
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;

    height: 100px;

    #logo{
        height: 70px;

        img{
            height: 100%;
        }
    }
    
    #links-container{
        display: flex;
        flex-flow: row nowrap;
        gap: 25px;

        font-size: 0.7em;
        font-weight: bold;

        .link{
            padding: calc(100px / 2 - 0.7em - 2.8px) 0;
            cursor: pointer;

            &:hover{
                color: #0288f9;
            }
        }
    }
}
</style>