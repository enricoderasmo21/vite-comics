<script>
export default{
    name: "AppMainCard",
    data() {
        return{

        }
    },
    props: {
        img: String,
        title: String,
    }
}
</script>

<template>
    <a href="#" class="card">
        <img :src="img" alt="">
        <div class="title"> {{ title }} </div>
    </a>

</template>

<style scoped lang="scss">
.card{
    margin-bottom: 30px;

    width: 150px;
    height: 220px;

    color: white;

    .title{
        font-size: 0.7em;
        font-weight: bold;
    }

    img{
        width: 100%;
        height: 100%;
    }

}

</style>