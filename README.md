<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Luvella | Luxury Ice Cream</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=Pacifico&family=Playfair+Display:wght@600;700;800&display=swap" rel="stylesheet">

<style>

/* =====================================================
   GLOBAL
===================================================== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

:root{
    --pink:#ef5b98;
    --pink2:#ff91bb;
    --purple:#9270e9;
    --cream:#fffaf7;
    --dark:#442d3a;
    --text:#76636d;
    --white:#ffffff;
    --gold:#dca942;
}

body{
    font-family:'DM Sans',sans-serif;
    background:var(--cream);
    color:var(--dark);
    overflow-x:hidden;
}

img{
    display:block;
    width:100%;
}

a{
    text-decoration:none;
    color:inherit;
}


/* =====================================================
   NAVBAR
===================================================== */

.navbar{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:9999;

    display:flex;
    align-items:center;
    justify-content:space-between;

    padding:18px 7%;

    background:rgba(255,255,255,.92);
    backdrop-filter:blur(18px);

    border-bottom:1px solid rgba(239,91,152,.08);
}

.logo{
    font-family:'Pacifico',cursive;
    font-size:32px;
    color:var(--pink);
}

.logo span{
    color:var(--purple);
}

.nav-links{
    display:flex;
    align-items:center;
    gap:30px;
}

.nav-links a{
    font-size:14px;
    font-weight:700;
    transition:.3s;
}

.nav-links a:hover{
    color:var(--pink);
}

.nav-order{
    color:white !important;
    padding:12px 23px;
    border-radius:30px;

    background:linear-gradient(135deg,var(--pink),var(--purple));

    box-shadow:0 12px 28px rgba(239,91,152,.25);
}

.mobile-menu{
    display:none;
    font-size:28px;
    cursor:pointer;
}


/* =====================================================
   HERO
===================================================== */

.hero{
    min-height:100vh;

    padding:140px 7% 80px;

    display:flex;
    align-items:center;
    justify-content:space-between;

    background:
    radial-gradient(circle at 5% 15%,#ffe2ed,transparent 30%),
    radial-gradient(circle at 95% 20%,#e8ddff,transparent 32%),
    linear-gradient(135deg,#fffaf7,#ffffff);

    overflow:hidden;
}

.hero-content{
    width:52%;
    position:relative;
    z-index:3;
}

.hero-badge{
    display:inline-block;

    padding:10px 18px;

    background:#ffffff;

    border-radius:40px;

    color:var(--pink);

    font-size:13px;
    font-weight:800;

    box-shadow:0 10px 30px rgba(68,45,58,.08);

    margin-bottom:23px;
}

.hero h1{
    font-family:'Playfair Display',serif;

    font-size:76px;

    line-height:1.03;
}

.hero h1 span{
    display:block;

    font-family:'Pacifico',cursive;

    font-weight:400;

    background:linear-gradient(
        90deg,
        var(--pink),
        var(--purple)
    );

    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.hero-description{
    max-width:590px;

    color:var(--text);

    font-size:17px;

    line-height:1.8;

    margin:25px 0 30px;
}

.hero-buttons{
    display:flex;
    gap:14px;
    flex-wrap:wrap;
}

.btn{
    display:inline-block;

    padding:15px 28px;

    border-radius:50px;

    font-weight:800;

    transition:.3s;
}

.btn-primary{
    color:#fff;

    background:
    linear-gradient(
        135deg,
        var(--pink),
        var(--purple)
    );

    box-shadow:
    0 15px 32px rgba(239,91,152,.27);
}

.btn-primary:hover{
    transform:translateY(-4px);
}

.btn-light{
    background:white;

    box-shadow:
    0 10px 28px rgba(68,45,58,.09);
}

.btn-light:hover{
    transform:translateY(-4px);
}


/* =====================================================
   HERO ICE CREAM
===================================================== */

.hero-visual{
    width:45%;

    min-height:570px;

    display:flex;
    align-items:center;
    justify-content:center;

    position:relative;
}

.hero-circle{
    position:absolute;

    width:500px;
    height:500px;

    border-radius:50%;

    background:
    linear-gradient(
        145deg,
        #ffd6e7,
        #e3d9ff
    );
}

.hero-icecream{
    position:relative;
    z-index:3;

    width:400px;
    height:530px;

    object-fit:cover;

    border-radius:
    220px
    220px
    45px
    45px;

    box-shadow:
    0 35px 80px
    rgba(68,45,58,.25);

    animation:floatIce 4s ease-in-out infinite;
}

@keyframes floatIce{

    0%,100%{
        transform:translateY(0);
    }

    50%{
        transform:translateY(-14px);
    }

}

.hero-label{
    position:absolute;

    z-index:6;

    padding:13px 18px;

    background:rgba(255,255,255,.94);

    border-radius:18px;

    font-size:13px;

    font-weight:800;

    box-shadow:
    0 15px 35px
    rgba(68,45,58,.12);
}

.hero-label-one{
    left:0;
    top:100px;
}

.hero-label-two{
    right:0;
    bottom:100px;
}


/* =====================================================
   FEATURES
===================================================== */

.features{
    padding:35px 7%;
    background:white;
}

.feature-grid{
    display:grid;
    grid-template-columns:
    repeat(4,1fr);

    gap:20px;
}

.feature{
    text-align:center;
    padding:20px;
}

.feature-icon{
    width:62px;
    height:62px;

    display:flex;
    align-items:center;
    justify-content:center;

    margin:auto;

    border-radius:50%;

    background:#fff0f6;

    font-size:27px;
}

.feature h3{
    margin:13px 0 5px;
}

.feature p{
    color:#89747e;
    font-size:13px;
}


/* =====================================================
   SECTION
===================================================== */

section{
    padding:100px 7%;
}

.section-title{
    text-align:center;
    margin-bottom:55px;
}

.section-title small{
    font-family:'Pacifico',cursive;

    color:var(--pink);

    font-size:22px;
}

.section-title h2{
    font-family:'Playfair Display',serif;

    font-size:48px;

    margin-top:8px;
}

.section-title p{
    max-width:650px;

    margin:14px auto;

    color:var(--text);

    line-height:1.7;
}


/* =====================================================
   FLAVOR GRID
===================================================== */

.flavors{
    background:#fff8f4;
}

.flavor-grid{
    display:grid;

    grid-template-columns:
    repeat(3,1fr);

    gap:28px;
}

.flavor-card{
    position:relative;

    background:white;

    padding:13px;

    border-radius:28px;

    box-shadow:
    0 15px 45px
    rgba(68,45,58,.08);

    transition:.4s;

    overflow:hidden;
}

.flavor-card:hover{
    transform:translateY(-10px);

    box-shadow:
    0 25px 60px
    rgba(68,45,58,.15);
}


/* CLEAN IMAGE BOX */

.flavor-image-box{
    width:100%;
    height:270px;

    overflow:hidden;

    border-radius:21px;

    background:#f8f5f2;
}

.flavor-image{
    width:100%;
    height:100%;

    object-fit:cover;

    transition:.5s;
}

.flavor-card:hover .flavor-image{
    transform:scale(1.05);
}


.flavor-info{
    padding:20px 8px 9px;
}

.flavor-info h3{
    font-family:'Playfair Display',serif;

    font-size:24px;
}

.flavor-info p{
    color:var(--text);

    font-size:13px;

    line-height:1.6;

    margin:8px 0 15px;
}

.flavor-bottom{
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.price{
    color:var(--pink);

    font-size:20px;

    font-weight:800;
}

.add-btn{
    width:43px;
    height:43px;

    border:0;

    border-radius:50%;

    color:white;

    background:
    linear-gradient(
        135deg,
        var(--pink),
        var(--purple)
    );

    font-size:22px;

    cursor:pointer;

    transition:.3s;
}

.add-btn:hover{
    transform:
    rotate(90deg)
    scale(1.1);
}

.tag{
    position:absolute;

    top:25px;
    left:25px;

    z-index:4;

    padding:7px 12px;

    background:white;

    color:var(--pink);

    border-radius:20px;

    font-size:10px;

    font-weight:900;

    box-shadow:
    0 8px 20px
    rgba(0,0,0,.12);
}


/* =====================================================
   STORY
===================================================== */

.story{
    display:flex;

    align-items:center;

    gap:75px;

    background:white;
}

.story-image{
    width:50%;
}

.story-image img{
    height:570px;

    object-fit:cover;

    border-radius:38px;

    box-shadow:
    0 25px 60px
    rgba(68,45,58,.15);
}

.story-content{
    width:50%;
}

.story-content small{
    font-family:'Pacifico',cursive;

    color:var(--pink);

    font-size:22px;
}

.story-content h2{
    font-family:'Playfair Display',serif;

    font-size:50px;

    line-height:1.15;

    margin:12px 0 20px;
}

.story-content p{
    color:var(--text);

    line-height:1.8;

    margin-bottom:16px;
}

.stats{
    display:flex;

    gap:45px;

    margin-top:30px;
}

.stat h3{
    color:var(--pink);

    font-size:30px;
}

.stat p{
    font-size:12px;
}


/* =====================================================
   PREMIUM OFFER
===================================================== */

.offer{
    margin:65px 7%;

    padding:70px;

    border-radius:40px;

    color:white;

    position:relative;

    overflow:hidden;

    background:
    linear-gradient(
        120deg,
        rgba(239,91,152,.98),
        rgba(146,112,233,.98)
    );
}

.offer h2{
    max-width:680px;

    font-family:'Playfair Display',serif;

    font-size:50px;
}

.offer p{
    max-width:570px;

    line-height:1.7;

    margin:15px 0 25px;
}

.offer .btn{
    background:white;

    color:var(--pink);
}

.offer-decoration{
    position:absolute;

    right:40px;
    bottom:-60px;

    font-size:190px;

    opacity:.13;
}


/* =====================================================
   REVIEWS
===================================================== */

.reviews{
    background:#fff8f4;
}

.review-grid{
    display:grid;

    grid-template-columns:
    repeat(3,1fr);

    gap:25px;
}

.review{
    background:white;

    padding:30px;

    border-radius:25px;

    box-shadow:
    0 12px 35px
    rgba(68,45,58,.07);
}

.stars{
    color:#e6ac39;

    font-size:18px;
}

.review > p{
    color:var(--text);

    line-height:1.7;

    margin:17px 0;
}

.customer{
    display:flex;

    align-items:center;

    gap:12px;
}

.customer img{
    width:48px;
    height:48px;

    border-radius:50%;

    object-fit:cover;
}

.customer h4{
    font-size:14px;
}

.customer span{
    color:#9a858f;

    font-size:11px;
}


/* =====================================================
   CONTACT
===================================================== */

.contact{
    background:white;

    text-align:center;
}

.contact-box{
    max-width:900px;

    margin:auto;

    padding:65px 30px;

    border-radius:38px;

    background:
    linear-gradient(
        135deg,
        #ffe4ef,
        #eee8ff
    );
}

.contact-box h2{
    font-family:'Playfair Display',serif;

    font-size:45px;
}

.contact-box p{
    color:var(--text);

    margin:12px auto 25px;
}

.email-box{
    max-width:550px;

    margin:auto;

    display:flex;

    padding:7px;

    background:white;

    border-radius:50px;

    box-shadow:
    0 10px 30px
    rgba(68,45,58,.08);
}

.email-box input{
    flex:1;

    border:0;
    outline:0;

    padding:14px 20px;

    font-family:inherit;
}

.email-box button{
    border:0;

    padding:14px 24px;

    border-radius:50px;

    color:white;

    font-weight:800;

    background:
    linear-gradient(
        135deg,
        var(--pink),
        var(--purple)
    );

    cursor:pointer;
}


/* =====================================================
   FOOTER
===================================================== */

footer{
    background:#422c38;

    color:white;

    padding:70px 7% 25px;
}

.footer-grid{
    display:grid;

    grid-template-columns:
    2fr 1fr 1fr 1.3fr;

    gap:45px;
}

.footer-logo{
    font-family:'Pacifico',cursive;

    font-size:34px;

    color:#ff82b7;
}

.footer-about p{
    max-width:360px;

    color:#d8c8d0;

    line-height:1.7;

    margin:15px 0 20px;
}

.socials{
    display:flex;
    gap:10px;
}

.social{
    width:40px;
    height:40px;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:50%;

    background:rgba(255,255,255,.1);

    transition:.3s;
}

.social:hover{
    background:var(--pink);

    transform:translateY(-4px);
}

footer h3{
    margin-bottom:17px;
}

footer ul{
    list-style:none;
}

footer li{
    color:#d8c8d0;

    margin:10px 0;

    font-size:13px;
}

.copyright{
    text-align:center;

    border-top:
    1px solid
    rgba(255,255,255,.1);

    padding-top:22px;

    margin-top:50px;

    color:#ae9ca5;

    font-size:12px;
}


/* =====================================================
   ANIMATION
===================================================== */

.reveal{
    opacity:0;

    transform:translateY(35px);

    transition:1s;
}

.reveal.active{
    opacity:1;

    transform:translateY(0);
}


/* =====================================================
   RESPONSIVE
===================================================== */

@media(max-width:1000px){

    .hero{
        flex-direction:column;

        text-align:center;
    }

    .hero-content,
    .hero-visual{
        width:100%;
    }

    .hero-description{
        margin-left:auto;
        margin-right:auto;
    }

    .hero-buttons{
        justify-content:center;
    }

    .hero-visual{
        margin-top:55px;
    }

    .feature-grid{
        grid-template-columns:
        repeat(2,1fr);
    }

    .flavor-grid{
        grid-template-columns:
        repeat(2,1fr);
    }

    .story{
        flex-direction:column;
    }

    .story-image,
    .story-content{
        width:100%;
    }

    .review-grid{
        grid-template-columns:1fr;
    }

    .footer-grid{
        grid-template-columns:
        repeat(2,1fr);
    }

}


@media(max-width:700px){

    .navbar{
        padding:15px 6%;
    }

    .mobile-menu{
        display:block;
    }

    .nav-links{
        display:none;

        position:absolute;

        top:68px;
        left:0;

        width:100%;

        padding:25px;

        background:white;

        flex-direction:column;

        box-shadow:
        0 15px 30px
        rgba(0,0,0,.08);
    }

    .nav-links.show{
        display:flex;
    }

    .hero{
        padding:
        120px
        6%
        60px;
    }

    .hero h1{
        font-size:49px;
    }

    .hero-visual{
        min-height:470px;
    }

    .hero-circle{
        width:330px;
        height:330px;
    }

    .hero-icecream{
        width:290px;
        height:420px;
    }

    .hero-label{
        font-size:11px;
    }

    section{
        padding:75px 6%;
    }

    .section-title h2,
    .story-content h2{
        font-size:38px;
    }

    .feature-grid,
    .flavor-grid{
        grid-template-columns:1fr;
    }

    .story-image img{
        height:430px;
    }

    .offer{
        margin:40px 5%;

        padding:45px 25px;
    }

    .offer h2{
        font-size:37px;
    }

    .offer-decoration{
        font-size:110px;

        right:-10px;
    }

    .stats{
        gap:20px;

        flex-wrap:wrap;
    }

    .email-box{
        flex-direction:column;

        border-radius:20px;
    }

    .email-box button{
        border-radius:15px;
    }

    .footer-grid{
        grid-template-columns:1fr;
    }

}

</style>

</head>


<body>


<!-- =====================================================
     NAVIGATION
===================================================== -->

<nav class="navbar">

    <a href="#home" class="logo">
        Luv<span>ella</span>
    </a>

    <div class="mobile-menu"
         onclick="toggleMenu()">
        ☰
    </div>

    <div class="nav-links"
         id="navLinks">

        <a href="#home">
            Home
        </a>

        <a href="#flavors">
            Flavors
        </a>

        <a href="#story">
            Our Story
        </a>

        <a href="#reviews">
            Reviews
        </a>

        <a href="#contact">
            Contact
        </a>

        <a href="#flavors"
           class="nav-order">
            Order Now 🍦
        </a>

    </div>

</nav>


<!-- =====================================================
     HERO
===================================================== -->

<section class="hero"
         id="home">

    <div class="hero-content reveal">

        <div class="hero-badge">
            ✨ Luxury Ice Cream Parlour
        </div>

        <h1>

            Taste the

            <span>
                beautiful side
                of ice cream.
            </span>

        </h1>

        <p class="hero-description">

            Premium handcrafted ice cream made
            with rich creamy textures and delicious
            flavors. Discover your perfect scoop
            at Luvella.

        </p>

        <div class="hero-buttons">

            <a href="#flavors"
               class="btn btn-primary">

                Explore Flavors 🍨

            </a>

            <a href="#story"
               class="btn btn-light">

                Discover Luvella →

            </a>

        </div>

    </div>


    <div class="hero-visual reveal">

        <div class="hero-circle"></div>

        <!-- CLEAN ICE CREAM PHOTO -->

        <img
        class="hero-icecream"
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQjRiYzwJ_KU59Tg2aKLK0_h-LYCPXcSJ1Wi9x4CMlfDw&s=10
        "
        alt="Luxury Gourmet Ice Cream">

        <div class="hero-label hero-label-one">
            🍦 Premium Scoops
        </div>

        <div class="hero-label hero-label-two">
            ⭐ 4.9 Loved by Customers
        </div>

    </div>

</section>


<!-- =====================================================
     FEATURES
===================================================== -->

<div class="features">

    <div class="feature-grid">

        <div class="feature">

            <div class="feature-icon">
                🥛
            </div>

            <h3>
                Rich & Creamy
            </h3>

            <p>
                Smooth premium texture.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                🍓
            </div>

            <h3>
                Quality Flavors
            </h3>

            <p>
                Carefully selected ingredients.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                ✨
            </div>

            <h3>
                Freshly Made
            </h3>

            <p>
                Crafted for every scoop.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                💗
            </div>

            <h3>
                Made With Love
            </h3>

            <p>
                Sweet moments guaranteed.
            </p>

        </div>

    </div>

</div>


<!-- =====================================================
     FLAVORS
===================================================== -->

<section class="flavors"
         id="flavors">

    <div class="section-title">

        <small>
            The Luvella Collection
        </small>

        <h2>
            Choose Your Flavor
        </h2>

        <p>
            Explore our carefully selected collection
            of creamy, delicious and luxurious ice cream.
        </p>

    </div>


    <div class="flavor-grid">


        <!-- STRAWBERRY -->

        <div class="flavor-card">

            <div class="tag">
                BEST SELLER
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSYNphlLAt9Q_KbLMcGvvZbwKToyLO0y4g4ViM9rBNmUQ&s=10"
                alt="Strawberry Bliss Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Strawberry Bliss
                </h3>

                <p>
                    Creamy strawberry ice cream
                    with a rich fruity finish.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 450
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Strawberry Bliss')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- CHOCO -->

        <div class="flavor-card">

            <div class="tag">
                POPULAR
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSFbUdLJZ-YeS4i0H6PhqM1c0QotBAbz5hr5ASvjfYOuQ&s=10"
                alt="Choco Dream Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Choco Dream
                </h3>

                <p>
                    Deep chocolate flavor with
                    a smooth creamy texture.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 520
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Choco Dream')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- VANILLA -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRIR7eUR9Q_CPHFKLIvAdp2BsD7Sh_SFM0MjUTfa_y9EA&s=10"
                alt="Vanilla Love Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Vanilla Love
                </h3>

                <p>
                    Classic silky vanilla ice cream
                    with a delicate creamy finish.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 400
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Vanilla Love')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- MANGO -->

        <div class="flavor-card">

            <div class="tag">
                FAVORITE
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQK2IicDzCfHcNyTkpZLvJyLeu2pYLxJBjKTOgbGMW6nQ&s=10">

            </div>

            <div class="flavor-info">

                <h3>
                    Mango Magic
                </h3>

                <p>
                    Tropical creamy mango flavor
                    with a bright fruity taste.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 480
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Mango Magic')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- COOKIE -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqKlOeRxjX8tLp41yKJN4j6Pe8AHCF9Ae6vuvf8vQ3gw&s=10"
                alt="Cookie Cream Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Oreo Ice-Cream
                </h3>

                <p>
                    Creamy cookie ice cream
                    with delicious crunchy pieces.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 500
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Cookie Cream')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- CARAMEL -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src=https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTR8N3XTt1_bXZnowIxAvXIYS5NVJEXlisya9Ly90OC4vdwi_aoWzLsJi8&s=10
               
                alt="Caramel Swirl Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Caramel Swirl
                </h3>

                <p>
                    Silky caramel ice cream
                    with luxurious caramel swirls.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 550
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Caramel Swirl')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- BLUEBERRY -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQPCQfPGwDeWslweBqsArsBvnAtyG4Zil4Go8OIQq-xDA&s=10"
                alt="Blueberry Scoop Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Blueberry Scoop
                </h3>

                <p>
                    Smooth blueberry ice cream
                    with a rich berry flavor.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 490
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Blueberry Scoop')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- KUNAFA -->

        <div class="flavor-card">

            <div class="tag">
                SIGNATURE
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWcJH_kaXi_mUtt3InOQAWKpEa_QKmq2JCnRcNVMWSjA&s=10"
                alt="Kunafa Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Kunafa Ice Cream
                </h3>

                <p>
                    Creamy dessert-inspired ice cream
                    with a luxurious Middle Eastern touch.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 650
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Kunafa Ice Cream')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- PISTACHIO -->

        <div class="flavor-card">

            <div class="tag">
                PREMIUM
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSkl0rx_bK2WmxEEYysrXprNttNq2dd0QYXkoUwBymXDA&s=10"
                alt="Pistachio Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Pistachio
                </h3>

                <p>
                    Rich nutty pistachio ice cream
                    with a smooth creamy texture.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 580
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Pistachio')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- BUTTER PECAN -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRlKjXEg5OBm2MrExma3n4GFTzKqt4FGbsnaVCKUUh2bw&s=10"
                alt="Butter Pecan Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Butter Pecan
                </h3>

                <p>
                    Rich buttery ice cream
                    with roasted pecan flavor.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 590
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Butter Pecan')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- RASPBERRY -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTlgZYOt9R5B2rRnrdtnNQEckw5UEmCU0V-yQ2TqJkrpA&s=10"
                alt="Raspberry Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                   Black Raspberry
                </h3>

                <p>
                    Bright raspberry flavor
                    with a smooth fruity finish.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 480
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Raspberry')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- PEACH -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://langschocolates.com/wp-content/uploads/2025/07/Keto-peach-ice-cream.png"
                alt="Peach Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Peach
                </h3>

                <p>
                    Soft fruity peach ice cream
                    with a fresh creamy taste.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 470
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Peach')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- COCONUT -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://www.lifenovo.co/wp-content/uploads/2023/07/Ice-Cream-scaled.jpg"
                alt="Coconut Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Coconut
                </h3>

                <p>
                    Smooth tropical coconut ice cream
                    with a refreshing finish.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 460
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Coconut')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- ALMOND -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRNSpwlbBy3R_cucGoUNyaPfSWsr9J9hlHRFFUF7MkoDA&s=10"
                alt="Almond Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Almond Joy Coconut Ice-Cream Bar
                </h3>

                <p>
                    Smooth almond cream with
                    delicate roasted nut notes.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 540
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Almond')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- HAZELNUT -->

        <div class="flavor-card">

            <div class="tag">
                NEW
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://static.vecteezy.com/system/resources/thumbnails/071/785/186/small/luxurious-hazelnut-ice-cream-sundae-dripping-with-caramel-in-a-crystal-glass-photo.jpg"
                alt="Hazelnut Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Hazelnut
                </h3>

                <p>
                    Roasted hazelnut ice cream
                    with rich nutty flavor.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 590
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Hazelnut')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- RED VELVET -->

        <div class="flavor-card">

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://curlygirlkitchen.com/wp-content/uploads/2022/12/Red-Velvet-Cake-Ice-Cream-Swirl-White-Cream-Cheese-No-Churn-Christmas-016.jpg"
                alt="Red Velvet Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Red Velvet
                </h3>

                <p>
                    Velvety creamy ice cream
                    inspired by classic red velvet.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 600
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Red Velvet')">
                        +
                    </button>

                </div>

            </div>

        </div>


        <!-- BELGIAN CHOCOLATE -->

        <div class="flavor-card">

            <div class="tag">
                LUXURY
            </div>

            <div class="flavor-image-box">

                <img
                class="flavor-image"
                src="https://ninja-icecream.com/wp-content/uploads/2026/03/recette-belgian-chocolate-facon-haagen-dazs-800x530.png"
                alt="Belgian Chocolate Ice Cream">

            </div>

            <div class="flavor-info">

                <h3>
                    Belgian Chocolate
                </h3>

                <p>
                    Deep luxurious chocolate ice cream
                    with an intense cocoa finish.
                </p>

                <div class="flavor-bottom">

                    <span class="price">
                        Rs. 650
                    </span>

                    <button
                    class="add-btn"
                    onclick="addFlavor('Belgian Chocolate')">
                        +
                    </button>

                </div>

            </div>

        </div>


    </div>

</section>


<!-- =====================================================
     STORY
===================================================== -->

<section class="story"
         id="story">

    <div class="story-image">

        <img
        src="https://gelatomargherita.swiss/wp-content/uploads/sites/66/2024/10/selection-of-different-ice-cream-scoops.jpg"
        alt="Luxury Ice Cream">

    </div>


    <div class="story-content">

        <small>
            The Luvella Story
        </small>

        <h2>
            Simple ingredients.
            Beautiful scoops.
        </h2>

        <p>
            Luvella is all about turning a simple
            scoop of ice cream into a beautiful
            experience.
        </p>

        <p>
            From classic vanilla and chocolate
            to pistachio, kunafa and Belgian
            chocolate, every flavor is created
            to feel rich, creamy and special.
        </p>

        <p>
            Come for one scoop and leave with
            a new favorite.
        </p>

        <a href="#flavors"
           class="btn btn-primary">

            Explore Our Flavors

        </a>

        <div class="stats">

            <div class="stat">

                <h3>17+</h3>

                <p>
                    Flavors
                </p>

            </div>


            <div class="stat">

                <h3>10K+</h3>

                <p>
                    Happy Customers
                </p>

            </div>


            <div class="stat">

                <h3>4.9★</h3>

                <p>
                    Rating
                </p>

            </div>

        </div>

    </div>

</section>


<!-- =====================================================
     OFFER
===================================================== -->

<div class="offer">

    <h2>
        One scoop is never enough.
    </h2>

    <p>
        Try your favorite Luvella flavor today
        and enjoy 20% OFF your first order.
    </p>

    <a href="#flavors"
       class="btn">

        Order Your Scoop

    </a>

    <div class="offer-decoration">
        🍦
    </div>

</div>


<!-- =====================================================
     REVIEWS
===================================================== -->

<section class="reviews"
         id="reviews">

    <div class="section-title">

        <small>
            Sweet Reviews
        </small>

        <h2>
            Loved One Scoop at a Time
        </h2>

        <p>
            What our ice cream lovers say
            about their Luvella experience.
        </p>

    </div>


    <div class="review-grid">


        <div class="review">

            <div class="stars">
                ★★★★★
            </div>

            <p>
                “Strawberry Bliss is so creamy
                and delicious. Definitely my
                favorite flavor!”
            </p>

            <div class="customer">

                <img
                src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=crop&w=200&q=80"
                alt="Customer">

                <div>

                    <h4>
                        Ayesha
                    </h4>

                    <span>
                        Happy Customer
                    </span>

                </div>

            </div>

        </div>


        <div class="review">

            <div class="stars">
                ★★★★★
            </div>

            <p>
                “Belgian Chocolate tastes
                incredibly rich and smooth.
                Absolutely loved it.”
            </p>

            <div class="customer">

                <img
                src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=200&q=80"
                alt="Customer">

                <div>

                    <h4>
                        Hamza
                    </h4>

                    <span>
                        Chocolate Lover
                    </span>

                </div>

            </div>

        </div>


        <div class="review">

            <div class="stars">
                ★★★★★
            </div>

            <p>
                “Kunafa Ice Cream is something
                completely different. Creamy,
                rich and amazing.”
            </p>

            <div class="customer">

                <img
                src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=200&q=80"
                alt="Customer">

                <div>

                    <h4>
                        Sarah
                    </h4>

                    <span>
                        Luvella Fan
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =====================================================
     CONTACT
===================================================== -->

<section class="contact"
         id="contact">

    <div class="contact-box">

        <h2>
            Join the Luvella Club 🍦
        </h2>

        <p>
            Get new flavor announcements,
            special offers and sweet surprises.
        </p>

        <div class="email-box">

            <input
            type="email"
            id="email"
            placeholder="Enter your email">

            <button onclick="subscribe()">

                Join Now

            </button>

        </div>

    </div>

</section>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

    <div class="footer-grid">


        <div class="footer-about">

            <div class="footer-logo">
                Luvella
            </div>

            <p>
                Luxury ice cream made for
                beautiful moments, delicious
                memories and happy hearts.
            </p>

            <div class="socials">

                <div class="social">
                    f
                </div>

                <div class="social">
                    ◎
                </div>

                <div class="social">
                    ▶
                </div>

                <div class="social">
                    ♥
                </div>

            </div>

        </div>


        <div>

            <h3>
                Explore
            </h3>

            <ul>

                <li>
                    <a href="#home">
                        Home
                    </a>
                </li>

                <li>
                    <a href="#flavors">
                        Flavors
                    </a>
                </li>

                <li>
                    <a href="#story">
                        Our Story
                    </a>
                </li>

                <li>
                    <a href="#reviews">
                        Reviews
                    </a>
                </li>

            </ul>

        </div>


        <div>

            <h3>
                Information
            </h3>

            <ul>

                <li>
                    Delivery
                </li>

                <li>
                    Privacy
                </li>

                <li>
                    Terms
                </li>

                <li>
                    FAQ
                </li>

            </ul>

        </div>


        <div>

            <h3>
                Visit Luvella
            </h3>

            <ul>

                <li>
                    📍 Islamabad, Pakistan
                </li>

                <li>
                    📞 +92 300 1234567
                </li>

                <li>
                    ✉ hello@luvella.com
                </li>

                <li>
                    🕐 11 AM – 11 PM
                </li>

            </ul>

        </div>

    </div>


    <div class="copyright">

        © 2026 Luvella Ice Cream.
        All Rights Reserved.

    </div>

</footer>


<script>

/* =====================================================
   MOBILE MENU
===================================================== */

function toggleMenu(){

    document
    .getElementById("navLinks")
    .classList.toggle("show");

}


/* =====================================================
   ADD FLAVOR
===================================================== */

function addFlavor(flavor){

    alert(
        "🍦 " +
        flavor +
        " added to your order!"
    );

}


/* =====================================================
   EMAIL
===================================================== */

function subscribe(){

    let email =
    document
    .getElementById("email")
    .value;

    if(email.trim()===""){

        alert(
            "Please enter your email address."
        );

        return;

    }

    alert(
        "Welcome to the Luvella Club! 🍦💗"
    );

    document
    .getElementById("email")
    .value="";

}


/* =====================================================
   SCROLL ANIMATION
===================================================== */

function reveal(){

    let items =
    document.querySelectorAll(".reveal");

    items.forEach(function(item){

        let position =
        item.getBoundingClientRect().top;

        if(
            position <
            window.innerHeight - 80
        ){

            item.classList.add("active");

        }

    });

}

window.addEventListener(
    "scroll",
    reveal
);

reveal();


/* =====================================================
   CLOSE MOBILE MENU
===================================================== */

document
.querySelectorAll(".nav-links a")
.forEach(function(link){

    link.addEventListener(
        "click",
        function(){

            document
            .getElementById("navLinks")
            .classList.remove("show");

        }
    );

});

</script>


</body>
</html>
