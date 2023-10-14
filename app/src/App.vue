<template>
  <HeaderComponent/>
  <IndexComponent/>
  <FooterComponent/>
  <HeaderComponent/>
  <ArticleComponent/>
  <FooterComponent/>
  <HeaderComponent/>
  <BlogDetailsComponent/>
  <FooterComponent/>
</template>

<script>
import IndexComponent from './components/IndexComponent.vue'
import ArticleComponent from './components/ArticleComponent.vue';
import BlogDetailsComponent from './components/BlogDetailsComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    IndexComponent, ArticleComponent, BlogDetailsComponent,
    HeaderComponent,
    FooterComponent
}
}
</script>

<style>

</style>
