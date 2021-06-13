<script>
export let fontsize;
export let articles;
export let idx;

let fontactualsize = fontsize[idx];


// console.log(fontsize,idx);
</script>

<style>
    .blog_article{
        line-height: 2;
        font-family: 'Montserrat', sans-serif;
    }
</style>

<div class="blog_article" style="font-size: {fontactualsize}px;">{articles}</div>