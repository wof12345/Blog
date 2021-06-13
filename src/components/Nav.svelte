<script>
    export let segment;

    // function log1(){
    //     console.log(segment);
    // }
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
    width: 100%;
}

.nav a:hover {
    background-size: 100% 2px, auto;
	opacity:.5;
}

.nav_item{
    margin: 1rem;
}

.nav_link--btn ,.nav_link--btn-inner{
    border: none;
    border-radius: 3rem;
    padding: 10px 25px;
    cursor: pointer;
    font-size: 1.2rem;
    background-color: rgba(39, 145, 238, 0.534);
    background-image: linear-gradient( black, black), none;
    background-size: 0 2px, auto;
    color: rgb(255, 255, 255);
    background-repeat: no-repeat;
    background-position: center bottom;
    transition: all 0.3s ease-out;
}

.display{
    display: none;
}

.nav_link--btn:hover ,.nav_link--btn-inner:hover{
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

.style_custom{
    position: sticky;
    top:0;
    height: 4rem;
    border-bottom: 1px solid rgba(148, 145, 145, 0.356);
    background-color: white;
}

@media screen and (max-width: 664px) {
		.nav_links {
            display: flex;
		    flex-direction: column;	
            padding: 0;
            margin: 0;
            width: 100%;
            text-align: center;
		}

        .link_cont{
            height: 45px;
            width: 30px;
            overflow: hidden;
            position: absolute;
            right: 10px;
            top:30px;
        }

        .nav_item{
            margin: 0px;
            width: 100%;
        }

        .nav_link--btn{
            display: none;
        }

        .nav_link--btn-inner{
            width: 100%;
        }

        .display{
            display: block;
        }

        .link_menu{
           display: block;
           width: 30px;
        }

        .link_cont:hover{
            height: 230px;
            width: 100px;
            background-color: rgb(255, 255, 255);
        }

        .nav a:hover,.nav_item:hover {
            background-size: 100% 2px, auto;
    	    opacity:.5;
            width: 100%;
            background-color: rgba(164, 166, 168, 0.295);
        }
	}

</style>

     <nav class="nav" class:style_custom={segment==='blog'}>
	 <img src="BlogLogo.png" alt="Blog logo" class="nav_logo" id="logo" />

     <div class="link_cont">
        <img class="link_menu" src="menu.svg" alt="">
            <ul class="nav_links">
                <li class="nav_item">
                    <a class="nav_link" href="/">link1</a>
                </li>
                <li class="nav_item">
                    <a class="nav_link" href="/">link2</a>
                </li>
                <li class="nav_item">
                    <a class="nav_link" href="/">link3</a>
                </li>
                <li class="nav_item">
                   <a class="nav_link" href="/">link4</a>
                </li>
            </ul>

            <button class="nav_link--btn-inner display">Any</button>
     </div>
			 <button class="nav_link--btn">Any</button>
    </nav>
