<script>
export let title;
export let subject;
export let short_detail;
export let author;
export let date;
</script>

<style>

.card_cont{
    width: 100%;
    min-width: 300px;
    margin: 0 5px;
}

.card{
    display: flex;
    flex-direction: column;
    transition: all .5s;
    border-radius: 6px;
    box-shadow: 0 5px 5px rgba(0, 0, 0, 0.123), 0px 0px 5px rgba(0, 0, 0, 0.11);
    background-color: white;
    text-decoration: none;
    
}

.card:hover{
    transform: translateY(10px);
    transform-style: preserve-3d;
    cursor: pointer;
}

.card_img{
    margin: 0px;
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 6px 6px 0 0 ;
}

.card_info{
    padding: 20px;
     margin: 0 auto;
    font-family: 'Montserrat', sans-serif;
}

.title{
    font-size: 20px;
    font-weight: 700;
}

.subject{
    margin-top: -20px;
    font-size: 14px;
}

.short_detail{
    font-size: 16px;
}

.author_date{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.author_date>*{
    font-size: 15px;
    color: rgba(39, 39, 39, 0.534);
}


</style>

<div class="card_cont">
<a class="card" href="blog">
    <img class="card_img" src="placeholder.jpg" alt="">

    <div class="card_info">
        <p class="title">{title}</p>
        <p class="subject">{subject}</p>

        <p class="short_detail">{short_detail}</p>

        <div class="author_date">
        <p class="author">{author}</p>
        <p class="date">{date}</p>
        </div>

    </div>
</a>
</div>