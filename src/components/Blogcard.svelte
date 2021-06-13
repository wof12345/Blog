<script>



</script>

<style>

.card_cont{
    width: 300px;
    margin: 0 auto;
}

.card{
    display: flex;
    flex-direction: column;
    transition: all .5s;
    border-radius: 10px;
    box-shadow: 0 5px 5px rgba(0, 0, 0, 0.123), 0px 0px 5px rgba(0, 0, 0, 0.11);
    background-color: white;
    text-decoration: none;
}

.card:hover{
    transform: translateY(20px);
    transform-style: preserve-3d;
    cursor: pointer;
}

.card_img{
    margin: 0px;
    width: 100%;
    border-radius: 10px 10px 0 0 ;
}

.card_info{
    padding: 20px;
}

.title{
    font-size: 18px;
    font-weight: bold;
}

.subject{
    margin-top: -20px;
    font-size: 14px;
}

.short_detail{
    font-size: 13px;
}

.author_date{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.author_date>*{
    font-size: 15px;
}



</style>

<div class="card_cont">
<a class="card" href="blog">
    <img class="card_img" src="placeholder.jpg" alt="">

    <div class="card_info">
        <p class="title">Random</p>
        <p class="subject">Computer</p>

        <p class="short_detail">This is a blog about computers.</p>

        <div class="author_date">
        <p class="author">Atif</p>
        <p class="date">6/29/2016</p>
        </div>

    </div>
</a>
</div>