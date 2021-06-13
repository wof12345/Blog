<script>
export let fontsize;
export let articles;

let fontactualsize = fontsize[articles];


console.log(fontsize,articles);
</script>

<style>
    .blog_article{
        line-height: 2;
    }
</style>

<div class="blog_article" style="font-size: {fontactualsize}px;">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur, in quasi soluta neque sed, perspiciatis quidem est fuga consequatur aspernatur adipisci et alias voluptates? Adipisci dolorem autem dignissimos ipsa sit.</div>