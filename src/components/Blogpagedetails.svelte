<script>
export let title;
export let short_detail;
export let subject;
export let author;
export let date;
</script>

<style>

.blog_details{
		margin: 30px;
		background-image: url('/placeholder.jpg');
		background-size: 100%;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		padding: 70px;
	}

	.blog_details>*{
		color: white;
		font-family: 'Montserrat', sans-serif;
	}	

    .blog_info{
        display: flex;
        justify-content: space-between;
    }

</style>

<section class="blog_details">

	<h1 class="title">{title}</h1>

	<h2 class="short_detail">{short_detail}</h2>

    <p class="subject">{subject}</p>

	<div class="blog_info">

		<p class="author">{author}</p>

		<p class="date">{date}</p>

	</div>
</section>