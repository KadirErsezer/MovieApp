<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lato&family=Lugrasimo&family=Roboto&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="buttonstyle.css">
    <style>
        
        * {box-sizing: border-box;}
        html {
            scroll-behavior: smooth;
        }
        body {
            margin: 0;
            font-family: 'Lato', sans-serif;
            background-color: azure;
        }
        h1, h2, h3 {
            font-family: 'Lugrasimo', cursive;
        }
        #showcase {
            background-image: url('darknight.jpeg');
            background-size: cover;
            height: 600px;
            width: 100%;
            padding: 20px;
            position: relative;
        }
        #showcase h1 {
            color: honeydew;
            position: absolute;
            top: 50%;
            margin: 0;
            left: 50%;
            transform: translate(-50% , -50%);
        }
        #how-it-works {
            padding: 10px;
        }
        #how-it-works h2 {
            color: #ED2B2A;
            font-size: 18;
            font-weight: 600;
            text-align: center;
        }
        #how-it-works p {
            text-align: center;
        }
        #main-header {
            background-color:#D71313;
            padding: 0px 10px;
            position: fixed;
            width: 100%;
            z-index: 1;
        }
        .main-header__logo {
            text-decoration: none;
            color: white;
            font-size: 18px;
            font-weight: 600;
            padding-left: 8px;
        }
        .main-nav {
            display: inline-block;
            width: calc(100% - 99px);
            text-align: right;
        }
        .main-nav__item {
            display: inline-block;
            text-decoration: none;
        }
        .main-nav__item a {
            color: white;
            text-decoration: none;
            padding: 0px 8px;
            font-size: 14px;
            font-weight: bold;
        }
        .main-nav__items a::before {
            content: '\2022';
            padding: 0px 7px;
        }
        .main-nav__item-login a {
            background-color: black;
            padding: 5px 16px;
            border-radius: 3px;
            text-align: center;
            border: 1px solid white;
        }
        .main-nav__item-login a:hover {
            background-color: white;
            color: black;
            border: 1px solid black;
            transition-duration: 0.6s;
        }
        .main-nav__item-login a::before {
            content: none;
        }

        .col-3 {
            display: inline-block;
            width: 33%;
            text-align: center;
            padding: 10px;
            margin-bottom: 40px;
            margin-top: 20px;
        }
        .col-3 h3 {
            color: #ED2B2A;
            font-size: 20px;
            font-weight: 600;
        }
        .col-3 i {
           color: #435B66;
        }
        .col-2 {
            display: inline-block;
            height: 350px;
            width: 50%;
            background-color: #435B66;
            vertical-align: top;
        }

        .features__left {
            background-image: url('pearlharbor.jpg');
            background-position: center;
            background-size: cover;
        }
        .features__right{
            color:honeydew;
            padding: 40px;
            vertical-align: top;
        }
        .features__right a {
            display: inline-block;
            margin-top: 20px;
            color:honeydew;
            text-decoration: none;
            background-color:#ED2B2A;
            color:honeydew;
            border: 2px solid #ED2B2A;
            border-radius: 4px;
            padding: 8px 16px;
            text-align: center;
        }
        .features__right a:hover {
            background-color: honeydew;
            color: #ED2B2A;
            border: 2px solid honeydew;
        }
        .plans-header {
            text-align: center;
            color: #ED2B2A;
            font-weight: 600;
        }
        .plan {
            text-align: center;
            padding: 5px;
            width: 33.3%;
            float: left;
            margin-bottom: 50px;
        }
        .inner-plan {
            background: #EEEEEE;
            padding: 25px 10px;
            border-radius: 5px;
            box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
            transition: box-shadow .5s;
        }
        .inner-plan:hover {
            box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 1) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
        }
        .section-title {
            text-align: center;
            padding-top: 40px;
            padding-bottom: 10px;
            margin-bottom: 40px;
        }
        .clearfix::after {
            content: "";
            display: block;
            clear: both;
        }
        .container {
            margin: 0 auto;
            width: 1000px;
        }
        .plan__badge {
            background-color: #ED2B2A;
            padding: 8px;
            border-radius: 5px;
            color: honeydew;
        }
        .plan__list {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }
        .plan__list li {
            margin: 6px 0px;
        }
        .recommended_plan {
            position: relative;
            top: -20px;
        }
       #backtotop {
        position: fixed;
        bottom: 10px;
        right: 10px;
       }
       #backtotop i {
        color: #ED2B2A;
        font-size: 45px;
       }
       #backtotop i:hover {
        color: #435B66;
        transition-duration: 0.3s;
       }

    </style>
</head>
<body id="body">

    <header id="main-header">
        <a href="#" class="main-header__logo">MovieApp</a>
        <nav class="main-nav">
            <ul class="main-nav__items">
                <li class="main-nav__item">
                    <a href="#">Home</a>
                </li>
                <li class="main-nav__item">
                    <a href="#">Movies</a>
                </li>
                <li class="main-nav__item main-nav__item-login">
                    <a href="#">Login</a>
                </li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section id="showcase">
            <h1></h1>
        </section>
        <section id="how-it-works">
            <div class="row">
            <h2>How it Works?</h2>
            <p>Welcome to MovieApp. Here we're present to all of the best movies in the film industry around the world</p>
            </div>

            <div class="row">
                <div class="col-3">
                    <i class="fa-solid fa-right-to-bracket fa-lg"></i>
                    <h3>Register</h3>
                    <p>Firstly, you should to create an acoount in that platform. Then you can choose a best plan for you membership.</p>
                </div>
                <div class="col-3">
                    <i class="fa-sharp fa-solid fa-cart-shopping fa-lg"></i>
                    <h3>Choose a Plan</h3>
                    <p>Now, you can choose a best plan for your membership. Next, you can pass to watch best movies with best quality</p>
                </div>
                <div class="col-3">
                    <i class="fa-solid fa-video fa-lg"></i>
                    <h3>Enjoy Movies</h3>
                    <p>You created an acoount and choosed a most suitable plan for you.Finally, you can enjoy movies what you want. Have a good time</p>
                </div>
            </div>
        </section>
        <section id="features">
            <div class="row-3">
                <div class="col-2 features__left"></div><div class="col-2 features__right">
                    <h3>Watch All Movies & TV Shows In 4K Quality</h3>
                    <p>We're prepared our web-site players in 4K Full Hd Quality for you. If you enjoy the real quality, please check your membership plan again.For the learn all features, please click on the button</p>
                    <a class="bttn-red" href="">View Features</a>
                </div>
            </div>
        </section>
        <section id="plans">
            <div class="row">
                <h2 class="section-title">Become a Premium Member</h2>
                <div class="container clearfix">
                    <div class="plan">
                        <div class="inner-plan">
                            <h2>Free</h2>
                            <h3>0/month</h3>
                            <ul class="plan__list">
                                <li>HD available</li>
                                <li>Unlimited Movies and TV shows</li>
                                <li>Watch on your phone & tablet</li>
                                <li>Download and watch offline</li>
                                <li>Screens you can watch</li>
                                <li>First Month Free</li>
                            </ul>
                            <div>
                                <button class="bttn-red">Choose Plan</button>
                            </div>
                        </div>
                    </div>
                    <div class="plan">
                        <div class="inner-plan recommended_plan">
                            <h2 class="plan__badge">Recommended</h2>
                            <h2>Basic</h2>
                            <h3>$9.99/month</h3>
                            <ul class="plan__list">
                                <li>HD available</li>
                                <li>Unlimited Movies and TV shows</li>
                                <li>Watch on your phone & tablet</li>
                                <li>Download and watch offline</li>
                                <li>Screens you can watch</li>
                                <li>First Month Free</li>
                            </ul>
                            <div>
                                <button class="bttn-red">Choose Plan</button>
                            </div>
                        </div>
                    </div>
                    <div class="plan">
                        <div class="inner-plan">                    
                            <h2>Premium</h2>
                            <h3>$19.99/month</h3>
                            <ul class="plan__list">
                                <li>HD available</li>
                                <li>Unlimited Movies and TV shows</li>
                                <li>Watch on your phone & tablet</li>
                                <li>Download and watch offline</li>
                                <li>Screens you can watch</li>
                                <li>First Month Free</li>
                            </ul>
                            <div>
                                <button class="bttn-red">Choose Plan</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <a href="#body" id="backtotop">
    <i class="fas fa-chevron-circle-up"></i>
    </a>

</body>
</html>
