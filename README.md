# Aditya-Kumar
Mini Project(Using HTML &amp; CSS)

I have made the project on Online Food delivery Site, using HTML and CSS.
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Best Online Food Delivery Service in India | MyOnlineMeal.com</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" media="screen and (max-width: 1170px)" href="css/phone.css">
    <link href="https://fonts.googleapis.com/css?family=Baloo+Bhai|Bree+Serif&display=swap" rel="stylesheet">
</head>

<body>
    <nav id="navbar">
        <div id="logo">
            <img src="logo.png" alt="MyOnlineMeal.com">
        </div>
        <ul>
            <li class="item"><a href="#home">Home</a></li>
            <li class="item"><a href="#services-container">Services</a></li>
            <li class="item"><a href="#coverage-section">Our Coverage</a></li>
            <li class="item"><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>

    <section id="home">
        <h1 class="h-primary">Welcome to Delicious Food</h1>
        <p>Grill and chill!. </p>
        <p>We at Delicious Food provide Food catering, Bulk order,Home Delivery etc. </p>
        <button class="btn">Order Now</button>
    </section>

    <section id="services-container">
        <h1 class="h-primary center">Our Services</h1>
        <div id="services">
            <div class="box">
                <img src="img/catering.png" alt="">
                <h2 class="h-secondary center">Food Catering</h2>
                <p class="center">We have one of the best quality of  caterers, who are available for catering for any event like Marriage,parties etc.</p>
            </div>
            <div class="box">
                <img src="img/bulk.png" alt="">
                <h2 class="h-secondary center">Bulk Ordering</h2>
                <p class="center">We at Delicious Food also provide bulk orders to our customers at Reasonable cost.</p>
            </div>
            <div class="box">
                <img src="img/3.png" alt="">
                <h2 class="h-secondary center">Faster Home Delivery</h2>
                <p class="center">We gurantee the delivery of your food at you doorstep within 45 mins of time period.</p>
            </div>
            <div class="box">
                <img src="img/vegetable.jpg" alt="">
                <h2 class="h-secondary center">Fresh Vegetable & Fruits</h2>
                <p class="center">We Provide all types of fresh vegetable and fruits at your doorstep .</p>
            </div>
            
        </div>
    </section>
    <section id="client-section">
        <h1 class="h-primary center">The Major City We Cover</h1>
        <div id="clients">
            <div class="client-item">
                <img src="img/delhi.jpg" alt="Our Client">
                <p class="center">Delhi</p>
            </div>
            <div class="client-item">
                <img src="img/mumbai.jpg" alt="Our Client">
                <p class="center">Mumabi</p>
            </div>
          
            <div class="client-item">
                <img src="img/pune.jpg" alt="Our Client">
                <p class="center">Pune</p>
            </div>
            <div class="client-item">
                <img src="img/hyderabad.jpg" alt="Our Client">
                <p class="center">Hyderabad</p>
            </div>
            <div class="client-item">
                <img src="img/kolkata.jfif" alt="Our Client">
                <p class="center">Kolakata</p>
            </div>
        </div>
        
        

    </section>

    <section id="contact">
        <h1 class="h-primary center">Contact Us</h1>
        <div id="contact-box">
            <form action="">
                <div class="form-group">
                    <label for="name">Name: </label>
                    <input type="text" name="name" id="name" placeholder="Enter your name">
                </div>
                <div class="form-group">
                    <label for="email">Email: </label>
                    <input type="email" name="name" id="email" placeholder="Enter your email">
                </div>
                <div class="form-group">
                    <label for="phone">Phone Number: </label>
                    <input type="phone" name="name" id="phone" placeholder="Enter your phone">
                </div>
                <div class="form-group">
                    <label for="message">Message: </label>
                    <textarea name="message" id="message" cols="20" rows="10"></textarea>
                </div>
            </form>
        </div>
        <div class="center">
            <button class="btn">Submit</button>
        </div>
    </section>

    <footer>
        <div class="center">
            Copyright &copy; www.deliciousfood.com. All rights reserved!
        </div>
    </footer>
</body>

</html>









CSS CODE


/* CSS Reset */
*{
    margin: 0;
    padding: 0;
}

html{
    scroll-behavior: smooth;
}

/* CSS Variables */
:root{
    --navbar-height: 59px;
}

/* Navigation Bar */
#navbar{
    display: flex;
    align-items: center;
    position: sticky;
    top: 0px;
}

#navbar::before{
    content: "";
    background-color: black;
    position: absolute;
    top:0px;
    left:0px;
    height: 100%;
    width:100%;
    z-index: -1;
    opacity: 0.7;
}

/* Navigation Bar: Logo and Image */
#logo{
    margin: 10px 34px;
}

#logo img{
    height: 59px;
    margin: 3px 6px;
}


/* Navigation Bar: List Styling */

#navbar ul{
    display: flex;
    font-family: 'Baloo Bhai', cursive;
}

#navbar ul li{ 
    list-style: none;
    font-size: 1.3rem;
}

#navbar ul li a{
    color: white;
    display: block;
    padding: 3px 22px;
    border-radius: 20px;
    text-decoration: none;
}

#navbar ul li a:hover{
    color: black;
    background-color: white;
}

/* Home Section */
#home{
    display: flex;
    flex-direction: column;
    padding:3px 200px;
    height: 550px;
    justify-content: center;
    align-items: center;
}

#home::before{ 
    content: "";
    position: absolute;
    background: url('../bg.jpg') no-repeat center center/cover;
    height: 642px;
    top:0px;
    left:0px;
    width: 100%;
    z-index: -1;
    opacity:0.89;
}

#home h1{
    color:white;
    text-align: center;
    font-family: 'Bree Serif', serif;
}

#home p{
    color:white;
    text-align: center;
    font-size: 1.5rem;
    font-family: 'Bree Serif', serif;
}
/* Services Section */
#services{
    margin: 34px;
    display: flex;
}
#services .box{ 
    border: 2px solid brown;
    padding: 34px;
    margin: 2px 55px;
    border-radius: 28px;
    background: #f2f2f2;
    margin-bottom: 20px;
}

#services .box img{ 
   height: 160px;
   margin: auto;
   display: block;
}

#services .box p{
    font-family: 'Bree Serif', serif;

} 

/* Clients Section */
#client-section{ 
    position: relative;
}

#client-section::before{
 content: "";
 position: absolute;
 background: url('../bg.jpg');
 width: 100%;
 height: 100%;
 z-index: -1;
 opacity: 0.3;
}

#clients{
    display: flex;
    justify-content: center;
    align-items: center;
}

.client-item{
    padding: 34px;
}

#clients img{
    height: 124px;
}


/* Contact Section */
#contact{
    position: relative;
}
#contact::before{
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: -1;
    opacity: 0.7;
    background: url('../contact.jpg') no-repeat center center/cover;

}
#contact-box{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 34px;
}
#contact-box input, 
#contact-box textarea{
    width: 100%;
    padding: 0.5rem;
    border-radius: 9px;
    font-size: 1.1rem;
} 

#contact-box form{
    width: 40%;
}

#contact-box label{
   font-size: 1.3rem;
   font-family: 'Bree Serif', serif;

}


footer{
    background: black;
    color: white;
    padding: 9px 20px;
}

/* Utility Classes */
.h-primary{
    font-family: 'Bree Serif', serif;
    font-size: 3.8rem;
    padding: 12px;
}

.h-secondary{
    font-family: 'Bree Serif', serif;
    font-size: 2.3rem;
    padding: 12px;
}

.btn{
    padding: 6px 20px;
    border: 2px solid white;
    background-color: brown;
    color: white;
    margin: 17px;
    font-size: 1.5rem;
    border-radius: 10px;
    cursor:pointer;
}

.center{
    text-align: center;
}




Phone CSS for Responsive
/* CSS Reset */
*{
    margin: 0;
    padding: 0;
}

html{
    scroll-behavior: smooth;
}

/* CSS Variables */
:root{
    --navbar-height: 59px;
}

/* Navigation Bar */
#navbar{
    display: flex;
    align-items: center;
    position: sticky;
    top: 0px;
}

#navbar::before{
    content: "";
    background-color: black;
    position: absolute;
    top:0px;
    left:0px;
    height: 100%;
    width:100%;
    z-index: -1;
    opacity: 0.7;
}

/* Navigation Bar: Logo and Image */
#logo{
    margin: 10px 34px;
}

#logo img{
    height: 59px;
    margin: 3px 6px;
}


/* Navigation Bar: List Styling */

#navbar ul{
    display: flex;
    font-family: 'Baloo Bhai', cursive;
}

#navbar ul li{ 
    list-style: none;
    font-size: 1.3rem;
}

#navbar ul li a{
    color: white;
    display: block;
    padding: 3px 22px;
    border-radius: 20px;
    text-decoration: none;
}

#navbar ul li a:hover{
    color: black;
    background-color: white;
}

/* Home Section */
#home{
    display: flex;
    flex-direction: column;
    padding:3px 200px;
    height: 550px;
    justify-content: center;
    align-items: center;
}

#home::before{ 
    content: "";
    position: absolute;
    background: url('../bg.jpg') no-repeat center center/cover;
    height: 642px;
    top:0px;
    left:0px;
    width: 100%;
    z-index: -1;
    opacity:0.89;
}

#home h1{
    color:white;
    text-align: center;
    font-family: 'Bree Serif', serif;
}

#home p{
    color:white;
    text-align: center;
    font-size: 1.5rem;
    font-family: 'Bree Serif', serif;
}
/* Services Section */
#services{
    margin: 34px;
    display: flex;
}
#services .box{ 
    border: 2px solid brown;
    padding: 34px;
    margin: 2px 55px;
    border-radius: 28px;
    background: #f2f2f2;
    margin-bottom: 20px;
}

#services .box img{ 
   height: 160px;
   margin: auto;
   display: block;
}

#services .box p{
    font-family: 'Bree Serif', serif;

} 

/* Clients Section */
#client-section{ 
    position: relative;
}

#client-section::before{
 content: "";
 position: absolute;
 background: url('../bg.jpg');
 width: 100%;
 height: 100%;
 z-index: -1;
 opacity: 0.3;
}

#clients{
    display: flex;
    justify-content: center;
    align-items: center;
}

.client-item{
    padding: 34px;
}

#clients img{
    height: 124px;
}


/* Contact Section */
#contact{
    position: relative;
}
#contact::before{
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: -1;
    opacity: 0.7;
    background: url('../contact.jpg') no-repeat center center/cover;

}
#contact-box{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 34px;
}
#contact-box input, 
#contact-box textarea{
    width: 100%;
    padding: 0.5rem;
    border-radius: 9px;
    font-size: 1.1rem;
} 

#contact-box form{
    width: 40%;
}

#contact-box label{
   font-size: 1.3rem;
   font-family: 'Bree Serif', serif;

}


footer{
    background: black;
    color: white;
    padding: 9px 20px;
}

/* Utility Classes */
.h-primary{
    font-family: 'Bree Serif', serif;
    font-size: 3.8rem;
    padding: 12px;
}

.h-secondary{
    font-family: 'Bree Serif', serif;
    font-size: 2.3rem;
    padding: 12px;
}

.btn{
    padding: 6px 20px;
    border: 2px solid white;
    background-color: brown;
    color: white;
    margin: 17px;
    font-size: 1.5rem;
    border-radius: 10px;
    cursor:pointer;
}

.center{
    text-align: center;
}



