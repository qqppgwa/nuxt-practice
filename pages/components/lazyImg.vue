<template>
    <!-- <figure v-for="(item,i) in imgs" :key="i"> -->
    <img v-lazy="imgSrc" class="aa" />
    <!-- </figure> -->
</template>
<script>

export default {
    props: {
        imgSrc: String
    },
    data () {
        return {

            // list: {
            //     input: '',
            //     done: false
            // }
        };
    },
    methods: {

    }
};
</script>
<style scoped>
img[lazy='loading'] {
    background-color: #ccc;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    animation-iteration-count: infinite;
    animation-name: placeHolderShimmer;
    animation-timing-function: linear;
    background: #f6f7f8;
    background: linear-gradient(to right, #f7f7f7 8%, #ececec 38%, #f7f7f7 63%);
    background-size: 100% 100%;
}
@keyframes placeHolderShimmer {
    0% {
        background-position: -515px 0;
    }
    100% {
        background-position: 515px 0;
    }
}
</style>
