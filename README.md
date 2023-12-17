<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA Compatible" content="IE-edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Personal Website Portfolio</title>
    <script src="https://kit.fontawesome.com/35c0d7a8b7.js" crossorigin="anonymous"></script>
</head>
<body>
    <div id="header">
        <div class="container">
            <nav>
                <img src="images/logo.png.png" class="logo">
                <ul>
                    <li><a href="#header">HOME</a></li>
                    <li><a href="#about">ABOUT</a></li>
                    <li><a href="#contact">CONTACT</a></li>
                </ul>
            </nav>
            <div class="header-text">
                <p>Computer Science Student</p>
                <h1>Hi, I'm Jan <br> Daniel Quemada</h1>
            </div>
        </div>
    </div>
    <!-----------------about-------------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="images/user.png.jpg">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>Hi, I'm Jan Daniel Quemada. I am a first year college Computer Science Student
                        in St. Peter's College, Iligan City. I am glad that you are here. 
                        Humans are prone to cynicism, and we often pull ourselves down by reflecting our negative qualities on a higher note. 
                        We need to reflect more on what we have planned and what we are looking forward to. 
                        One can choose to explore their meritorious capabilities, which can range from developing hobbies to polished talents. 
                        This, in turn, will also work to boost your motivation towards any goal you set for yourself.</p>
                        <div class="tab-titles">
                            <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                            <p class="tab-links" onclick="opentab('hobbies')">Hobbies</p>
                            <p class="tab-links" onclick="opentab('achievements')">Achievements</p>
                        </div>
                        <div class="tab-contents active-tab" id="skills">
                            <ul>
                                <li>COMMUNICATION :<br> Verbal, Written, and Public Speaking </li>
                                <li>TECHNOLOGY :<br> Social Media, Microsoft Productivity Tools </li>
                                <li>SOFT-SKILLS: <br> Teamwork, Punctuality, Leadership, Flexibility, Critical Thinking. </li>
                            </ul>
                        </div>
                        <div class="tab-contents" id="hobbies">
                            <ul>
                                <p>______________________________________________________________________________________</p>
                                <p>Hobbies: </p>
                                <li>-Reading Books</li>
                                <li>-Playing Basketball</li>
                                <li>-Playing Video Games</li>
                            </ul>
                        </div>
                        <div class="tab-contents" id="achievements">
                            <ul>
                                <p>______________________________________________________________________________________</p>
                                <p>Achievments: </p>
                                <li>MUSIC: <br>ACOUSTIC CHAMPION at Saint Therese Academy (2022-2023)</li>
                                <li>SPORTS: <br> VARSITY PLAYER (BASKETBALL) at Saint Therese Academy (2019-2020)</li>
                                <li>OVER-ALL: <br> PERFORMING ARTIST OF THE YEAR at Saint Therese Academy (2016-2017)</li>
                            </ul>
                        </div>
                </div>
            </div>
        </div>
    </div>
    <!----------------------contact----------------------->
    <div id="contact">
        <div class="container">
            <div class="row">
                <div class="contact-left">
                   <p>_______________________________________________________________________________________________________________________________</p>
                    <h1 class="sub-tittle">Contact Me</h1>
                    <p> <i class="fa-solid fa-paper-plane"></i>danieltuazon15@gmail.com</p>
                    <p> <i class="fa-solid fa-phone"></i>09465830729</p>
                    <div class="social-icons">
                        <a href="https://facebook.com/https://www.facebook.com/Dane.Quemada.1?mibextid=2JQ9oc"><i class="fa-brands fa-facebook"></i></a>
                        <a href="https://instagram.com/https://www.instagram.com/allfordawgs_?igshid=YzAwZjE1ZTI0Zg%3D%3D&utm_source=qr"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
</div>
    <script>

    var tablinks = document.getElementsByClassName("tab-links");
    var tabcontents = document.getElementsByClassName("tab-contnets");

    function opentab(tabname){
        for(tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for(tabcontent of tabcontents){
            tabcontent.classList.remove("active-tab");
        }
        event.currentTarget.classList.add("active-link");
        document.getElementById(tabname).classList.add("active-tab");
    }

    </script>
    *{
    margin: 0;
    padding: 0;
    font-family: 'Times New Roman', Times, serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth;
}
body{
    background: #080808;
    color: #fff;
}
#header{
    width: 100%;
    height: 100vh;
    background-image: url(images/background.png);
    background-size: contain;
    background-position: center;
}
.container{
    padding: 10px 10%;
}

nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo{
    width: 200px;
    border-radius: 15px;
    
}

nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}
nav ul li a{
    text-decoration: none;
    color: black;
    font-size: 18px;
    position: relative;
}
nav ul li a::after{
    content: '';
    width: 0%;
    height: 3px;
    background: black;
    position: absolute;
    right: 0;
    bottom: -6px;
    transition: 0.8s;
}
nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
}
.header-text h1{
    font-size: 60px;
    margin-top: 20px;
}
/*---------------about-----------*/
#about{
    padding: 80px 0;
    color: #fff;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width: 100%;
    height: 100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}

.sub-title{
    font-size: 60px;
    font-weight: 600;
    text-align: justify;
}

.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}

.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: white;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.8s;
}

.tab-links.active-link::after{
    width: 100%;
}

.tab-contents ul li{
list-style: none;
margin: 10px 0;
}

.tab-contents{
    display: none;
}
.tab-contents.active-tab{
    display: block;
}
/*-----------contact--------*/
.contact-left{
    flex-basis: 35%;
}
.contact-right{
    flex-basis: 80%;
}
.contact-left p{
    margin-top: 30px;
}
.contact-left p i{
    margin-right: 15px;
    font-size: 25px;
}
.social-icons{
    margin-top: 30px;
}
.social-icons a{
    text-decoration:none;
    font-size: 30px;
    margin-right: 15px;
    display: inline-block;
    transition: transform 0.6s;
}
.social-icons a:hover{
    transform: translateY(-5px);
}

</body>
</html>
