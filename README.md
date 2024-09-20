<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer"/>
    <link rel="stylesheet" href="./Assets/logo.png">
    <title>Spotify - web player : music for everyone</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>



<style>
    body{
    font-family: 'montserrat', sans-serif;
    margin: 0px;
    background-color: black;
    color: white;
    overflow: hidden;
}
.main{
    display: flex;
    height: 100vh;
    padding: 0.5rem;
}

.sidebar{
    background-color: black;
    width: 330px;
    border-radius: 1rem;
    margin-right: 0.5rem;

}

.maincontent{
background-color: rgb(39, 37, 37);
flex: 1;
overflow: auto;
border-radius: 1rem;  
padding: 0 1.5rem 0 1.5rem;
}

.musicplayer{
    background-color: black;
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 75px;
}
  a {
    text-decoration: none;
    color: white; 
}
.nav{
    background-color:  rgb(39, 37, 37);
    border-radius: 1rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100px;
    padding: 0.5rem  0.75rem;

}
.navoption{
    line-height: 2.5rem;
    opacity: 0.7;
    padding: 0.5rem 0.75rem;
}
.navoption:hover{
   
    opacity: 1;
}
.navoption i{
    font-size: 1.25rem;
}

.navoption a{
    font-size: 1rem;
    margin-left: 1rem;
}
.library{
    background-color: rgb(39, 37, 37);
    border-radius: 1rem;
    padding: 0.5rem  0.75rem;
    height: 100%;
    margin-top: 0.5rem;
    
}
.options{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.icons{
    font-size: 1.25rem;
    display: flex;
}
.icons i{
    opacity: 0.7;
    margin-right: 1rem;
}
.icons i:hover{
    opacity: 1;
}
.box{
    background-color: rgb(53, 53, 53);
    height: 8rem;
    border-radius: 0.75rem;
    margin: 0.75rem 0 1.75rem 0;
    padding: 0.75rem 1rem;
}
.p1{
    font-size: 1rem;
    font-weight: 600;
}
.p2{
    font-size: 0.85rem;
    opacity: 0.75;
}
.badge{
    background-color: white;
    border: none;
    border-radius: 100px;
    padding: 0.25rem 1rem;
    font-weight: 700;
    margin-top: 0.5rem;
    height: 2rem;
    width: fit-content;

}
.cardcontainer{
    display: flex;
    flex-wrap: wrap;
    margin-top: 1rem;
}


.card{
    background-color: rgb(53, 53, 53);
    width: 150px;
    border-radius: 0.25rem;
    padding: 1rem;
    margin-left: 1.5rem;
}
.card img{
    width: 100%;
    border-radius: 0.25rem;
    
}
.cardtitle{
    font-weight: 700;
}
.cardinfo{
    opacity: 0.7;
    font-size: 0.7rem;
}
.footer{
    height: 300px;
    align-items: center;
    justify-content: center;
    display: flex;
}
.line{
    width: 90%;
    height: 50%;   
    border-top: 1px solid white;
    opacity: 0.4;
    
}
</style>
</head>
<body>
    <div class="main">
        <div class="sidebar">

            <div class="nav">
                <div class="navoption">
                    <i class="fa-solid fa-house"></i>
                    <a href="#">Home</a>
                </div>
                <div class="navoption">
                    <i class="fa-solid fa-magnifying-glass"></i>
                    <a href="#">Search</a>
                </div>
            </div>
            <div class="library">
                <div class="options">
                    <div class="liboption navoption">
                        <i class="fa-solid fa-magnifying-glass"></i>
                        <a href="#">your library</a>
                    </div>
                    <div class="icons">
                        <i class="fa-solid fa-plus"></i>
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>
                <div class="libboxes">
                    <div class="box">
                        <p class="p1">Create your first playlist</p>
                        <p class="p2">its easy we'll help you</p>
                        <button class="badge">create playlist</button>
                    </div>
                    <div class="box">
                        <p class="p1">let's find some podcasts to follow</p>
                        <p class="p2">We'll keep you updated on new episodes</p>
                        <button class="badge">Browse Podcasts</button>
                    </div>
                </div>
            </div>
        
        </div>
        <div class="maincontent">

            
                <h2>Recently played</h2>
                <div class="cardcontainer">
                    <div class="card">
                        <img src="/new projects/MY PROJECTS/My projects/Assets/card1img.jpeg" alt="">
                        <p class="cardtitle">Top 50 globals</p>
                        <p class="cardinfo">your daily updates of most played tracks...</p>
                    </div>
                </div>
            
                <h2>Trending now near you</h2>
                <div class="cardcontainer">
                    <div class="card">
                        <img src="/new projects/MY PROJECTS/My projects/Assets/card2img.jpeg" alt="">
                        <p class="cardtitle">Top 50 globals</p>
                        <p class="cardinfo">your daily updates of most played tracks...</p>
                    </div>


                    <div class="card">
                        <img src="/new projects/MY PROJECTS/My projects/Assets/card3img.jpeg" alt="">
                        <p class="cardtitle">Top 50 globals</p>
                        <p class="cardinfo">your daily updates of most played tracks...</p>
                    </div>


                    <div class="card">
                        <img src="/new projects/MY PROJECTS/My projects/Assets/card4img.jpeg" alt="">
                        <p class="cardtitle">Top 50 globals</p>
                        <p class="cardinfo">your daily updates of most played tracks...</p>
                    </div>

                </div>

                <h2>Featured charts</h2>
                <div class="cardcontainer">
                    <div class="card">
                        <img src="/new projects/MY PROJECTS/My projects/Assets/card6img.jpeg" alt="">
                        <p class="cardtitle">Top songs India</p>
                        <p class="cardinfo">your daily updates of most played tracks...</p>
                    </div>
       
        </div>
              
        <div class="footer">
            <div class="line"></div>
        </div>
    </div>
    
    <div class="musicplayer">
        <div class="album"></div>
        <div class="player"></div>
        <div class="controls"></div>
    </div>

</body>
</html>
