<script>
</script>

<style>

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    z-index: 100;
	font-size: 1.2rem;
}


.nav_logo {
    height: 90px;
    transition: all 0.3s;
}

.link_cont{
    transition: all .5s;
}

.link_cont>*{
margin:10px 0 ;
}

.nav_links {
    display: flex;
    list-style: none;
    font-weight: 400;
    list-style: none;
}

.nav a {
    text-decoration: none;
    transition: color 0.2s ease-out;
    background-image: linear-gradient( black, black), none;
    background-size: 0 2px, auto;
    background-repeat: no-repeat;
    background-position: center bottom;
    transition: all 0.3s ease-out;
}

.nav a:hover {
    background-size: 100% 2px, auto;
	opacity:.5;
}

.nav_item{
    margin: 2rem;
}

.nav_link--btn ,.nav_link--btn-inner{
    border: none;
    border-radius: 3rem;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 1.2rem;
    background-color: rgba(91, 164, 228,.45);
    background-image: linear-gradient( black, black), none;
    background-size: 0 2px, auto;
    color: aliceblue;
    background-repeat: no-repeat;
    background-position: center bottom;
    transition: all 0.3s ease-out;
}

.display{
    display: none;
}

.nav_link--btn:hover {
	color:black;
    background-color: white;
    background-size: 100% 2px, auto;
}

.link_menu{
    display: none;
}

.link_menu:hover{
    cursor: pointer;
    background-color: rgba(201, 205, 209, 0.418);
}

@media screen and (max-width: 614px) {
		.nav_links {
            display: flex;
		    flex-direction: column;	
            padding: 0;
            margin: 0;
            align-items: center;
		}

        .link_cont{
            height: 45px;
            width: 40px;
            overflow: hidden;
            position: absolute;
            right: 10px;
            top:30px;
        }

        .nav_item{
            margin: 0px;
        }

        .nav_link--btn{
            display: none;
        }

        .display{
            display: block;
        }

        .link_menu{
           display: block;
           width: 40px;
        }

        .link_cont:hover{
            height: 250px;
            width: 100px;
            background-color: rgba(240, 248, 255, 0.199);
        }
	}

</style>

     <nav class="nav">
	 <img src="BlogLogo.png" alt="Blog logo" class="nav_logo" id="logo" />

     <div class="link_cont">
        <img class="link_menu" src="menu.svg" alt="">
            <ul class="nav_links">
                <li class="nav_item">
                    <a class="nav_link" href="#">link1</a>
                </li>
                <li class="nav_item">
                    <a class="nav_link" href="#">link2</a>
                </li>
                <li class="nav_item">
                    <a class="nav_link" href="#">link3</a>
                </li>
                <li class="nav_item">
                   <a class="nav_link" href="#">link4</a>
                </li>
            </ul>

            <button class="nav_link--btn-inner display">Any</button>
     </div>
			 <button class="nav_link--btn">Any</button>
    </nav>
