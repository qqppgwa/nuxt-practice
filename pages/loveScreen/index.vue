<template>
    <section>
        <figure v-for="(item,i) in lage" :key="i">
            <lazyImg :imgSrc="item" />
        </figure>

    </section>
</template>
<script>
import lazyImg from '~/pages/components/lazyImg.vue';
export default {
    data () {
        return {
            lage:
                ['https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_03.jpg?alt=media&token=36825e46-15e3-4afa-b30b-7cd8504191c9',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_05.jpg?alt=media&token=b2303ef5-d60e-49ab-8e48-2dce0ad6a57c',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_06.jpg?alt=media&token=0138fa10-8ff3-411f-9f97-7fa55f939dea',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_08.jpg?alt=media&token=a1d16b52-b3a1-4f44-903d-89d4a22d0c49',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_16.jpg?alt=media&token=0cde67cb-778d-4bf8-84d9-5cab06649b56']
        };
    },
    components: {
        lazyImg
    },
    methods: {

    }
};
</script>
<style scoped>
section {
    width: 100%;
}
figure {
    width: 90%;
    margin: auto;
    max-width: 800px;
}
img {
    width: 100%;
}
</style>
