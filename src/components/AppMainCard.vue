<script>
export default{
    name: "AppMainCard",
    data() {
        return{

        }
    },
    props: {
        // img: String,
        title: String,
    }
}
</script>

<template>
    <div class="card">
        <img src="/img/test-thumb.jpg" alt="">
        <div class="title"> {{ title }} </div>
    </div>

</template>

<style scoped lang="scss">
.card{
    width: 150px;

    color: white;

    .title{
        font-size: 0.7em;
        font-weight: bold;
    }

    img{
        width: 100%;
    }

}

</style>