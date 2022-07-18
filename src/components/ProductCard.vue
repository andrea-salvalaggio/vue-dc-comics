<template>
    <div>
        <div class="img-container">
            <img :src="imgUrl" :alt="title">
        </div>
        <h6 class="mb-0"> {{ title }} </h6>
    </div>
</template>

<script>
export default {
    props: {
        'imgUrl': String,
        'title': String,
    },
}
</script>

<style lang="scss" scoped>
    .img-container{
        width: 200px;
        height: 200px;
        margin: 0 auto;

        img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
        }
    }

    h6{
        color: white;
        text-transform: uppercase;
        font-weight: 400;
        margin-top: 10px;
    }

</style>