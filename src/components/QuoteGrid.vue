<template>
    <div class="row">
        <app-quote v-for="(quote, idx) in quotes" @click.native="deleteQuote(idx)">{{ quote }}</app-quote>
    </div>
</template>

<script>
    import Quote from './Quote.vue'
    export default {
        name: "QuoteGrid",
        props: ['quotes'],
        components: {
          appQuote: Quote
        },
        methods: {
          deleteQuote(idx) {
            this.$emit('quoteDeleted', idx);
          }
        }
    }
</script>

<style scoped>

</style>
