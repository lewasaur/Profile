<template>
    <a @click="scrollView(scrollSelector)">
        {{ title }}
    </a>

</template>

<script>
//https://github.com/rigor789/vue-scrollto
//https://stackoverflow.com/questions/40730116/scroll-to-bottom-of-div-with-vue-js SCROLL BUTTOM OF DIV
//https://github.com/rigor789/vue-scrollto?ref=madewithvuejs.com vue scrollto library - npm + indexhtml include
//https://forum.vuejs.org/t/scroll-to-content-in-another-component/99235/2 scroll to content in another component
//https://laracasts.com/series/practical-vue-components/episodes/1 anchor tag header??

export default {
    name: 'NavLink',
    props: {
        title: {
            type: String,
            default: 'link'
        },
        scrollSelector: {
            type: String,
            default: ''
        }
    },
    methods: {
        scrollView(selector) {
            document.querySelector(selector).scrollIntoView({behavior: "smooth"})
        }
    }
}
</script>

<style scoped>
    a {
        cursor: pointer;
    }
</style>