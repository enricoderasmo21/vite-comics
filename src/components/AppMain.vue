<script>
export default{
    data(){
        return{
            message: "--> Content goes here <--",
        }
    }
}
</script>

<template>

        <section class="sec-one">
            <div class="container-centered">
    
                <div id="test"> {{ message }} </div>
                
            </div>  
        </section>

</template>

<style scoped lang="scss">

.sec-one{
    display: flex;
    flex-direction: row;
    align-items: center;

    min-height: 100px;

    background-color: #1c1c1c;
    
    #test{
        font-size: 1.6em;
        font-weight: bold;

        color: white;
    } 
}
</style>