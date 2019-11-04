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
                ['https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_09.jpg?alt=media&token=0751b930-f491-4ce2-811a-5eec52a846ad',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_11.jpg?alt=media&token=1d01f369-3e31-420e-b9cf-35d1dfcebe29',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_12.jpg?alt=media&token=2dbfd13b-8246-4fdf-bc35-0b3b8d875a1c',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_23.jpg?alt=media&token=09910956-a9c8-43a5-ae93-5ef9a5f4c0cd',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_24.jpg?alt=media&token=d8f86d4e-6ad2-4149-9cb9-b7a668ae702e',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FLageScreen%2Fresume%20and%20porfolio_%E9%A0%81%E9%9D%A2_15.jpg?alt=media&token=2ca6a7ca-7d03-4064-a540-8cada7290108']
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
