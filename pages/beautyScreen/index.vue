<template>
    <section>
        <h1> mobile web screenshot</h1>
        <div class="mobile">

            <figure v-for="(item,i) in m" :key="i">
                <lazyImg :imgSrc="item" />
            </figure>
        </div>
        <hr>
        <h1> desktop web screenshot</h1>
        <figure class="desk">
            <lazyImg :imgSrc="d" />
        </figure>

    </section>
</template>
<script>
import lazyImg from '~/pages/components/lazyImg.vue';
export default {
    data () {
        return {
            m:
                ['https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-search-2019-07-12-16_34_58.png?alt=media&token=67c3d4c6-6b01-4b27-9283-360e93d0e1ff',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-search-2019-07-12-16_35_18.png?alt=media&token=0a05a8ab-6322-417f-b753-ef260a307940',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-search-2019-07-12-16_35_30.png?alt=media&token=783a181c-ad92-4859-b184-47440a9d9328',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-search-l-2019-07-12-16_36_07.png?alt=media&token=cdd4a282-8794-47ee-ad95-bc4009cef335',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-uweb-beautybee-notification-2019-07-12-16_50_16.png?alt=media&token=1908b893-071c-4757-a3c6-8ed7ca4f77ee',

                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-uweb-beautybee-setting-2019-07-12-16_41_30.png?alt=media&token=1ee6885c-b00b-4e45-9814-b7bb8ad3247e',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-uweb-beautybee-setting-2019-07-12-16_41_49%20(1).png?alt=media&token=06ec0acf-e35b-4589-a65a-9126484008e6',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-search-l-2019-07-12-16_35_42.png?alt=media&token=55a699cd-a3f4-4876-a3cc-a327abfe2b2b',
                    'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-uweb-beautybee-post-5d1acb02dfd6fd22ec14fad2-2019-07-12-16_42_30.png?alt=media&token=0cddc514-3cbb-4a8c-8b4d-f839319d3282',],
            d: 'https://firebasestorage.googleapis.com/v0/b/froggychat-ce2ec.appspot.com/o/image%2FbeautyScreen%2Fscreencapture-localhost-8000-2019-07-12-16_38_43%20(1).png?alt=media&token=cac10135-8e41-4a35-a72b-7e8a0dc0bd1d'

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

    background-color: antiquewhite;
}
.mobile {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    max-height: 3000px;
}
figure {
    width: 20%;
    margin: 20px;
}
img {
    width: 100%;
}
figure.desk {
    width: 80%;
    max-width: 800px;
    margin: auto;
}
h1 {
    text-align: center;
    padding: 20px;
}
</style>
