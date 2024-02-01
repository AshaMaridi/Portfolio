<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="pp.css">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
        <title>My Personal Portfolio</title>
      
    </head>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@900&family=Poppins:wght@300;400;500;600;700&display=swap');

:root {
    --header-height: 6rem;


    --first-color: hsl(350, 98%, 64%);
    --title-color: hsl(0, 0%, 100%);
    --text-color: hsl(0, 0%, 77%);
    --body-color: hsl(0, 0%, 6%);
    --container-color: hsl(0, 0%, 10%);
    ---border-color: hsl(0, 0%, 100%, 0.2);


    --body-font: 'Poppins', sans-serif;
    --second-font: 'Montserrat', sans-serif;

    --big-font-size: 4.5rem;
    --h1-font-size: 3.75rem;
    --h2-font-size: 1.75rem;
    --h3-font-size: 1.5rem;
    --normal-font-size: 1.25rem;
    --small-font-size: 1rem;
    --smaller-font-size: 0.75rem;

    --weight-300: 300;
    --weight-400: 400;
    --weight-500: 500;
    --weight-600: 600;
    --weight-700: 700;
    --weight-900: 900;

    --transition: cubic-bezier(0.05, 0.2, 0.1, 1);

    --radius: 0.5rem;

    --z-tooltip: 10;
    --z-fixed:  100;
}

@media screen and (max-width: 992px){
 :root{
    --h2-font-size: ;
    --h3-font-size: ;
    --normal-font-size: ;
    --small-font-size: ;
    --smaller-font-size: ;
 }
};
    
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

input,
textarea,
body{
    color: var(--text-color);
    font-family: var(--body-font);
    font-size: var(--normal-font-size);
    font-weight: var(--weight-300);
}

body{
    background-color: var(--body-color);
}

h1,
h2,
h3{
    color: var(--title-color);
    font-weight: var(--weight-700);
}

ul{
    list-style: none;
}
a{
    text-decoration: none;
}
p{
    line-height: 1.67em;
}
img{
    max-width: 100%;
}

textarea,
input{
    background-color: transparent;
    border: none;
    outline: none;
}
.container{
    max-width: 1260px;
    margin-inline: auto;
    padding-inline: 0.75rem;
}
.grid{
    display: grid;
    gap: 1.75rem;
}
.section{
    padding-block: 8rem;
}
.section__title{
    font-size: var(--h1-font-size);
    margin-bottom: 1rem;
}
.section__title,
.section__description {
    text-align: center;
}
.section__description{
    max-width: 600px;
    margin-inline: auto;
    margin-bottom: 3.75rem;
}
.home{
    padding-block: 16rem 16rem 16rem;
}
.home__container{
    
    margin-top: 200px;
    margin-left: 300px;
    margin-bottom: 120px;
    grid-template-columns: 7fr 7fr 7fr;
    align-items: center;
    text-align: center;
}
.home__subtitle{
    
    font-size: var(--small-font-size);
    font-weight: var(--weight-400);
    letter-spacing: 0.25rem;
    margin-bottom: 1.25rem;
    display: block;
}
.home__title{
    font-family: var(--first-font);
    font-size: var(--big-font-size);
    font-weight: var(--weight-900);
}
.home__container span{
    color: crimson;
}
/*-----------------------*/
#About{
    padding: 80px 0;
    color: #ababab;
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
    margin-top: 40%;
    width: 100%;
    height: 60%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}
.sub-title{
    font-size: 60px;
    font-weight: var(--weight-600);
    color: #fff;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    color: #fff;
    margin-right: 50px;
    font-size: 18px;
    font-weight: var(--weight-500);
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contents ul li{
    list-style: none;
    margin: 10px 0;
    color: #fff;
    font-size: 20px;
}
.tab-contents ul li span{
    color: crimson;
    font-size: 15px;
}
.tab-contents{
    display: none;
}
.tab-contents.active-tab{
    display: block;
}
.services__container{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}
.services__item{
    margin-top: 30px;
    margin-bottom: 30px;
    margin-right: 30px;
    margin-left: 40px;
    padding: 3.5rem 2.5rem;
    border-radius: var(--radius);
    background-color: var(--container-color);  
}
.services__item h3{
    text-align: center;
    text-shadow: 1px 1px 5px crimson, 0 0 25px hotpink, 3px 0 5px darkblue;
    text-decoration: underline;
}
.services__item h3 p{
    text-align: center;
    text-justify: auto;
}
.portfolio{
    background-color: var(--container-color);
}
.portfolio__container{ 
    grid-template-columns: repeat(3, 1fr);
}
.portfolio__items{
    position: relative;
    cursor: pointer;
    border-radius: var(--radius);
    overflow: hidden;   
}
.portfolio__items::after,
.portfolio__data{  
    position: absolute;
    transition: all 0.65s var(--transition);   
}
.portfolio__img{
    
    width: 50%;
    vertical-align: middle;
    transition: all 1s var(--transition);
}
.portfolio__items::after{
    content: '';
    inset: 0;
    background: linear-gradient(180deg, transparent, var(--first-color));
    opacity: 0;
}
.portfolio__data{
    
    inset-inline: 1rem;
    bottom: 5rem;
    text-align: center;
    z-index: var(--z-tooltip);
}
.portfolio__data,
.portfolio__subtitle,
.portfolio__description{
    color: var(--title-color);
    opacity: 0.9;
}
.portfolio__data,
.portfolio__subtitle{
    font-size: var(--small-font-size);
    margin-bottom: .5rem;
}
.portfolio__data,
.portfolio__title{
    font-size: var(--h2-font-size);
    font-weight: var(--weight-600);
    margin-bottom: 0.7rem;
}
.portfolio__data,
.portfolio__description{
    font-weight: var(--weight-400);
    display: none;
}
.portfolio__items:hover::after{
    opacity: 2;
}
.portfolio__items:hover .portfolio__img{
    transform: scale(1.1);
}
.portfolio__items:hover .portfolio__description{
    display: block;
}
.portfolio__items:hover .portfolio__data{
    transform: translateY(-2rem);
}
.contact__container{
    grid-template-columns: repeat(2,1fr);
    align-items: center;
    column-gap: 4rem;
}
.contact__description,
.contact_input{
    font-weight: var(--weight-400);
}
.contact__description{
    margin-bottom: 3rem;
}
.contact__description a{
    color: var(--title-color);
    font-weight: var(--weight-500);
}
.contact_input{
    border: 2px solid var(---border-color);
    padding: 0.6rem 1.25rem;
    width: 100%;
}
.contact-container{
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-color: #fff;
    box-shadow: #ababab;
}
.contact-left{
    margin: 150px;
    display: flex;
    flex-direction: column;
    align-items: start;
    gap: 20px;
    border-color: #ababab;
}
.contact-left-title{
    text-shadow: 1px 1px 5px crimson, 0 0 25px hotpink, 3px 0 5px darkblue;
    
}
.contact-left hr{
    border: none;
    width: 120px;
    height: 5px;
    background-color: rgb(177, 151, 156);
    border-radius: 10px;
    margin-bottom: 20px;
}
.contact-input{
    width: 400px;
    height: 50px;
    border: none;
    outline: none;
    font-weight: 500;
    border-radius: 50px;
    text-shadow: 1px 1px 5px crimson, 0 0 25px hotpink, 3px 0 5px darkblue;
}
.button{
    width: 10px;
    height: 10px;
    border-radius: 20px;
    text-shadow: 1px 1px 5px crimson, 0 0 25px hotpink, 3px 0 5px darkblue;   
}
  </style>
    <body>

        <main class="main">
            <section class="Home" id="Home">
                <i class="fa-solid fa-house fa-bounce" style="margin: 20px; padding: 10px; color: crimson;"></i>
                <i class="fa-solid fa-user fa-beat" style="margin: 20px; padding: 10px; color: crimson;"></i>
                <i class="fa-solid fa-layer-group fa-bounce" style="margin: 20px; padding: 10px; color: crimson;"></i>
                <i class="fa-solid fa-phone fa-shake" style="margin: 20px; padding: 10px; color: crimson;"></i>
                <div class="home__container container grid">
                    <div class="home__content">
                        <span class="home__subtitle">Welcome to my world.</span>
                        <h1 class="home __title">Hi, I'm Asha Latha <br> <span>Front-End-Developer.</span><br> Based in A.P</h1>
                    </div>
                    <img src="Home..jpg.jpeg" alt="" class="Home__img" style="border-radius: 50%; border: 0.75rem solid var(--container-color); margin-left: auto;">
                </div>
            </section>
        
        <!--About me-->
        <div id="About">
            <div class="container">
                <div class="row">
                    <div class="about-col-1">
                        <img src="about..jpg" style="border-radius: 150px;">
                    </div>
                    <div class="about-col-2">
                        <h1 class="sub-title" style="text-shadow:  1px 1px 5px crimson, 0 0 25px hotpink, 3px 0 5px darkblue;;">About Me</h1>
                        <p>In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content. Lorem ipsum may be used as a placeholder before final copy is available.</p>
                       
                        <div class="tab-titles">
                            <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                            <p class="tab-links" onclick="opentab('certifications')">Certifications</p>
                            <p class="tab-links" onclick="opentab('education')">Education</p>    
                        </div>

                        <div class="tab-contents active-tab" id="skills">
                            <ul>
                                <li><span>UI/UX</span><br>Designing App/Web Interfaces</li>
                                <li><span>Web Development</span><br>Web App Development</li>
                                <li><span>App Development</span><br>Building IOS/Android Apps</li>
                            </ul>
                        </div>
                 
                        <div class="tab-contents" id="certifications">
                            <ul>
                                <li><span>Synchro serve</span><br>Web development</li>
                                <li><span>Nichrome Company</span><br>Journal Enteries</li>
                                <li><span>DIET</span><br>APTET</li>
                            </ul>
                        </div>
                 
                        <div class="tab-contents" id="education">
                            <ul>
                                <li><span>B.Com Computers</span><br>St.Joseph's College For Women Edu(A)</li>
                                <li><span>DIET</span><br>Sri Vinayaka Venkateswara Educational institute</li>
                                <li><span>MEC</span><br>Sri Chaitnaya</li>
                            </ul>
                        </div>
                 
                    </div>
                </div>
            </div>
        </div>

        <section class="services section" id="services">
            <h2 class="section__title">My Awesome services</h2>
            <p class="section__description">In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content.</p>
        
            <div class="services__container">
            <div class="services__item">
                <i class="fa-solid fa-square-rss fa-shake" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 135px;"></i>
                <h3 class="service__title">Business Startagy</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>

            <div class="services__item">
                <i class="fa-solid fa-layer-group fa-bounce" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 135px;"></i>

                <h3 class="service__title">Web Development</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>

            <div class="services__item">
                <i class="fa-solid fa-user fa-beat" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 150px;"></i>
                <h3 class="service__title">User</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>

            <div class="services__item">
                <i class="fa-solid fa-desktop fa-bounce" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 135px;"></i>
                <h3 class="service__title">Mobile Development</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>


            <div class="services__item">
                <i class="fa-solid fa-users fa-beat" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 135px;"></i>
                <h3 class="service__title">Marketing & Reporting</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>

            <div class="services__item">
                <i class="fa-solid fa-desktop fa-bounce" style="color: crimson; font-size: xx-large; font-weight: 900; margin-left: 135px;"></i>
                <h3 class="service__title">Mobile Deveployment</h3>
                <p class="services__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
            </div>
         </div>
        </section>

        <section class="portfolio section" id="portfolio">
            <h2 class="section__title">My Latest Project</h2>
            <p class="section__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>

            <div class="portfolio__container container grid">
                <div class="portfolio__items">
                    <img src="Port.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>


                <div class="portfolio__items">
                    <img src="P2.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>


                <div class="portfolio__items">
                    <img src="P3.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>

                <div class="portfolio__items">
                    <img src="P4.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>

                <div class="portfolio__items">
                    <img src="P4.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>

                <div class="portfolio__items">
                    <img src="P4.png" alt="" class="portfolio__img" style="width: 300px; height: 215px;">
                </div>

                <div class="portfolio__data">
                    <p class="portfolio__subtitle">Development</p>
                    <h3 class="portfolio__title">web Design</h3>
                    <p class="portfolio__description">In publishing and graphic design, Lorem ipsum is a placeholder text</p>
                </div>

            </div>
        </section>
        
        <div class="contact-container">
            <form action="" class="contact-left">
                <div class="contact-left-title">
                    <h2>Get In Touch</h2>
                    <p>I'm open for freelancing, Please feel free to <br>call: <i class="fa-solid fa-phone fa-shake"></i>+91 1234567891.<br> Connect me on <br>E-mail: <i class="fa-solid fa-envelope fa-shake"></i>20AH623Asha@gmail.com</p>
                    <hr>
                </div>
                <input type="text" name="name" placeholder="Your Name" class="contact-input" required>
                <input type="email" name="email" placeholder="Your email" class="contact-input" required>
                <textarea name="Message" placeholder="Your Message" class="contact-input" required></textarea>
                <button type="submit">submit</button>
            </form>
            <div class="contact-right">
                <img src="Home..jpg.jpeg" alt="" style="float: left; margin-right: 350px; border-radius: 200px;">
            </div>
        </div>
    </main>
    <script src="pp.js">
  
var tablinks = document.getElementsByClassName('tab-links');
var tabcontents = document.getElementsByClassName('tab-contents');

function opentab(tabname){
    for(tablinks of tablinks){
        tablinks.classList.remove("active-link");
    }
    
    for(tabcontents of tabcontents){
        tabcontents.classList.remove("active-tab");
    }
        
    event.currentTarget.classList.add("active-link");
    document.getElementById(tabname).classList.add('active-tab');
    
}

    
    



    </script>        
    </body>
</html>
