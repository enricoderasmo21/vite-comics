<script>
export default{
    name: "MainCardItem",
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

    width: calc(100% / 6 - 45px / 6 * 3);

    color: white;

    .title{
        font-size: 0.7em;
        font-weight: bold;
    }

    img{
        width: 100%;

        aspect-ratio: 1/1;

        object-fit: cover;
        object-position: top;
    }

}

</style>