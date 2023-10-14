<template>
    <div class="banner">
        <div class="banner-block">
            <h1 class="banner-block__header">Articles & News</h1>
            <p class="banner-block__text">Home / Blog</p>
        </div>
    </div>
    <div class="post">
        <h1 class="post-header">Latest Post</h1>
        <div class="post-block">
            <img class="post-block__image" src="../assets/img/latestpost.png" alt="photo latest post">
            <div class="post-block__content">
                <h2 class="post-block__subheader">Low Cost Latest Invented Interior<br> Designing Ideas</h2>
                <p class="post-block__textfirst">Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis
                    dignissim
                    maximus.posuere in.Contrary to popular belief.</p>
                <p class="post-block__textsecond">Lorem Ipsum is not simply random text. It has roots in a piece of
                    classica.</p>
                <div class="post-block__date">
                    <p>26 December,2022</p>
                    <svg width="52" height="53" viewBox="0 0 52 53" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <circle cx="26" cy="26.5" r="26" fill="#F4F0EC" />
                        <path d="M23.771 33.1855L29.7139 26.4998L23.771 19.8141" stroke="#292F36" stroke-width="2"
                            stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                </div>
            </div>
        </div>
    </div>
    <div class="articles">
        <div class="articles-header">
            <h1 class="articles-header__head">Articles & News</h1>
        </div>
        <div id="app" class="articles-content">
            <CardComponent v-for="item in articles" :key="item.id" :article="item"/>
        </div>
        <div class="articles-pagination">
            <div class="articles-pagination__item">
                <svg width="53" height="52" viewBox="0 0 53 52" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="26.5" cy="26" r="25.5" stroke="#CDA274" />
                </svg>
                <p>01</p>
            </div>
            <div class="articles-pagination__item">
                <svg width="53" height="52" viewBox="0 0 53 52" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="26.5" cy="26" r="25.5" stroke="#CDA274" />
                </svg>
                <p>02</p>
            </div>
            <div class="articles-pagination__item">
                <svg width="53" height="52" viewBox="0 0 53 52" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="26.5" cy="26" r="25.5" stroke="#CDA274" />
                </svg>
                <p>03</p>
            </div>
            <div class="articles-pagination__item">
                <svg width="53" height="52" viewBox="0 0 53 52" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="26.5" cy="26" r="25.5" stroke="#CDA274" />
                    <path d="M23.5571 32L29.5 25.3143L23.5571 18.6286" stroke="#292F36" stroke-width="2"
                        stroke-linecap="round" stroke-linejoin="round" />
                </svg>
            </div>
        </div>
    </div>
    
</template>

<script>
    
    import img4 from "../assets/img/article1.png";
    import img5 from "../assets/img/article2.png";
    import img6 from "../assets/img/article3.png";
    import img7 from "../assets/img/article4.png";
    import img8 from "../assets/img/article5.png";
    import img9 from "../assets/img/article6.png";
import CardComponent from "./CardComponent.vue";
export default{
    data() {
        return {
            articles: [
                {
                    id: 1, img: img4, rectangle: "Kitchen Design", header1: "Let’s Get Solution For Building Construction", header2: "Work", date: "26 December,2022"
                },
                {
                    id: 2, img: img5, rectangle: "Living Design", header1: "Low Cost Latest Invented Interior Designing", header2: "Ideas.", date: "22 December,2022"
                },
                {
                    id: 3, img: img6, rectangle: "Interior Design", header1: "Best For Any Office & Business Interior ", header2: "Solution", date: "25 December,2022"
                },
                {
                    id: 4, img: img7, rectangle: "Kitchen Design", header1: "Let’s Get Solution For Building Construction ", header2: "Work", date: "26 December,2022"
                },
                {
                    id: 5, img: img8, rectangle: "Living Design", header1: "Low Cost Latest Invented Interior Designing ", header2: "Ideas.", date: "22 December,2022"
                },
                {
                    id: 6, img: img9, rectangle: "Interior Design", header1: "Best For Any Office & Business Interior ", header2: "Solution", date: "25 December,2022"
                },
            ],
        };
    },
    components: { CardComponent }
}
</script>