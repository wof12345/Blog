<script>
    export let segment;
    import { onMount } from 'svelte';

    // function log1(){
    //     console.log(segment);
    // }

    onMount(async () => {
        if(segment==='blog'){
	const nav = document.querySelector('.nav');
    const link = document.querySelector('.link_cont')

    window.addEventListener('scroll',function(){
        if(window.scrollY>=100){
            changestyle('2rem','10px');
    }else{
            changestyle('4rem','30px');
    }

    function changestyle(str1,str2){
        nav.style.height = str1;
        link.style.top = str2;
    }
    })

        }
	});
</script>

<style>

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    z-index: 100;
	font-size: 1.2rem;
    transition: all .5s;
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
    margin: 0 1rem;
}

.nav a:hover {
    background-size: 100% 2px, auto;
	opacity:.5;
}

.nav_link--btn ,.nav_link--btn-inner{
    border: none;
    border-radius: 10px;
    padding: 10px 25px;
    cursor: pointer;
    font-size: 1.2rem;
    background-color: rgba(39, 175, 238, 0.288);
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


@media screen and (max-width: 669px) {
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

        .nav a{
            margin:0;
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
            height: 214px;
            width: 140px;
            background-color: rgb(255, 255, 255);
            border-radius: 10px;
            box-shadow: 0 10px 10px rgba(0, 0, 0, 0.171);
        }

        .nav a:hover {
            background-size: 100% 2px, auto;
    	    opacity:.5;
            width: 100%;
            background-color: rgba(164, 166, 168, 0.295);
        }
	}

</style>

     <nav class="nav" class:style_custom={segment==='blog'}>
	 <img src="Logo.png" alt="Blog logo" class="nav_logo" id="logo" />

     <div class="link_cont">
        <img class="link_menu" src="menu.svg" alt="">
            <div class="nav_links">
                <a class="nav_link" href="/">Home</a>
                <a class="nav_link" href="/">About</a>
                <a class="nav_link" href="/">Contributions</a>
                <a class="nav_link" href="/">Projects</a>
            </div>

            <button class="nav_link--btn-inner display">Log in</button>
     </div>
			 <button class="nav_link--btn">Log in</button>
    </nav>
