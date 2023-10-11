<template>
  <IndexComponent/>
  <ArticleComponent/>
  <BlogDetailsComponent/>
</template>

<script>
import IndexComponent from './components/IndexComponent.vue'
import ArticleComponent from './components/ArticleComponent.vue';
import BlogDetailsComponent from './components/BlogDetailsComponent.vue';

export default {
  name: 'App',
  components: {
    IndexComponent, ArticleComponent, BlogDetailsComponent
  }
}
</script>

<style>

</style>
