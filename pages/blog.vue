<template>
    <section class="section">
        <div class="container">
            <div class="columns is-multiline">
                <div
                    class="column is-one-quarter"
                    v-for="(article, index) in articles"
                    :key="index">
                    <a :href="article.url" target="_blank">
                        <div class="card">
                            <div class="card-image">
                                <figure class="image is-square">
                                    <img :src="article.urlToImage" :alt="article.title">
                                </figure>
                            </div>
                            <div class="card-content">
                                <div class="content">{{ article.title }}</div>
                            </div>
                        </div>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        async asyncData({ app }) {
            const { articles } = await app.$axios.$get(
                `https://newsapi.org/v2/top-headlines?sources=reddit-r-all&apiKey=${
                    process.env.API_KEY
                }`
            );
            return { articles };
        }
    };
    // import axios from 'axios'
    // export default {
    //     data (){
    //         return {
    //             articles: []
    //         }
    //     },
    //     beforeMount(){
    //         this.getArticles(this.articles)
    //     },
    //     methods: {
    //         getArticles(arr){
    //             this.axios.get(
    //             `https://newsapi.org/v2/top-headlines?sources=reddit-r-all&apiKey=${
    //                 process.env.API_KEY
    //             }`).then(data => {
    //                 arr = data
    //             }).catch(e => {
    //                 console.log(e)
    //             });
    //             return arr
    //         }
    //     }
    // };
</script>