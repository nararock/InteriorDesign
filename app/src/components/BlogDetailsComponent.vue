<template>
    <HeaderComponent/>
    <div class="blog-banner"></div>
    <div id="articles">
        <ArticleItemComponent/>
    </div>
    <FooterComponent/>
</template>

<script>
import HeaderComponent from "./HeaderComponent.vue";
import FooterComponent from "./FooterComponent.vue";
import ArticleItemComponent from "./ArticleItemComponent.vue";
export default{
    components:{
        ArticleItemComponent, HeaderComponent,FooterComponent
    }
}
</script>