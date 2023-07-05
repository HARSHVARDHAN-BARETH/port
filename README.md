
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <script src="https://kit.fontawesome.com/b20b9e1db0.js" crossorigin="anonymous"></script>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="media.css">
</head>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&family=Roboto:wght@400;700&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root{
    --primary-text-color: #183b56;
    --secondary-text-color: #577592;
    --accent-color: #2294ed;
    --accent-color-dark: #1d69a3;
    --padding-inliine-section: 20px;
}
body{
    font-family: 'Poppins', sans-serif;
    background-color: #f8f8ff;
color: var(--primary-text-color);
}

h1{
    font-size: 3rem;;
}

h2{
    font-size: 2rem;
}

h3{
   font-size: 1.5rem;
}
p{
    font-family: 'Roboto', sans-serif;
    font-size: 1.25rem;
    color: var(--secondary-text-color);
    line-height: 1.8rem;
}
a{
    text-decoration: none;
    display: inline-block;
}
ul{
    list-style: none;
}
.logo{
    font-size: 26px;
    font-weight: 700;
}
.hover-link{
    color: var(--primary-text-color);
    font-size: 18px;
    font-weight: 600;
}
.active{
    color: var(--accent-color);
}
.hover-link:hover{
    color: var(--accent-color);

}
/*Utility Classes */
.container{
    max-width: 1180px;
    padding-inline: var(--padding-inliine-section);
    margin-inline: auto;
    overflow: hidden;
}
.flex{
    display: flex;
    align-items: center;
}
.primary-btn{
    background-color: var(--accent-color);
    border-radius: 6px;
    font-weight: 700;
    color: white !important;
    padding: 12px 24px;
    box-shadow: 0 0 2px var(--secondary-text-color);
    transition: 0.2s ease-out;
}
.primary-btn:hover{
    background-color: var(--accent-color-dark);
}
.secondary-btn{
    border: 0.5px solid var(--secondary-text-color);
    border-radius: 6px;
    font-weight: 700;
    color: var(--primary-text-color) !important;
    padding: 12px 24px;
    transition: 0.2s ease-out;
}
.secondary-btn:hover{
    color: var(--accent-color) !important;
}
/* header */
.main-nav{
    justify-content: space-between;
    margin-top: 20px;
}
.nav-links{
    flex-basis: 730px;
}
nav ul{
    justify-content: end;
    gap: 40px;
}
.nav-toggle{
    display: none;
}
/*Header section */
header{
    padding: 50px var(--padding-inliine-section) 0;
}
.header-section{
    justify-content: space-between;
    
}
.header-left{
    max-width: 40vw;
}
.header-left h2{
    margin-top: 20px;
}
.get-strated{
    margin-top: 20px;
}
.header-right img{
    width: 100%;
}

/* About Section */
.headings{
    text-align: center;
}
.about-section{
    justify-content: center;
    padding: 30px 20px 30px 20px;
    gap: 50px;
}
.about-left img{
   width: 300px;
}
.about-right{
    padding: 1px 34px;
  max-width: 36vw;
}
.btn{
    justify-content: flex-start;
    margin-left: 500px;
}
.cv{
    outline: none;
    border: none;
    font-weight: 700;
    width: 160px;
    height: 50px;
    cursor: pointer;
    padding: 12px 24px;
}
/*Projects */
.gallery{
    width: 900px;
    display: flex;
    overflow-x: scroll;
  }
  .gallery::-webkit-scrollbar{
    display: none;
  }
  .gallery div{
    width: 100%;
    display: grid;
    grid-template-columns: auto auto auto;
    grid-gap: 40px;
    padding: 10px;
    flex: none;
  }
  .gallery div img{
    width: 100%;
    
    transition: 0.5s;
  }
  .gallery-wrap{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 5% auto;
  }
  #backbtn, #nextbtn{
    width: 50px;
    cursor: pointer;
  }
  #backbtn{
    margin-right: 70px;
  }
  .gallery div img:hover{
   
    cursor: pointer;
    transform: scale(1.1);
  }
  

/* Skills Section */

.skills-section{
   padding: 50px 20px 30px 20px;
   justify-content: center;
    display: grid;
    grid-template-columns: auto auto auto ;
    column-gap: 50px;
    row-gap: 50px;
}
.skills-section img{
    width: 200px;
}
.skills-card{
    flex-direction: column;
    gap: 20px;
    max-width: 30%;
    text-align: center;
 }
 .skills-area {
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 40px;
    margin-top: 20px;
 }
/*education */

.time-line{
    position: relative;
    max-width: 1200px;
    margin: 100px auto;
  }
  .content-p{
    padding: 10px 50px;
    position: relative;
    border-radius: 20px;
    width: 50%;
   
  }
  .tex-box{
   padding: 20px 30px;
   background-color: #fff;
   position: relative;
   border-radius: 20px;
   font-size: 15px;
   border: 1px solid black;
  }
  .content-l{
    left: 0;
  }
  .content-r{
    left: 50%;
  }
  .content-p img{
    position: absolute;
    width: 40px;
    right: -20px;
    top: 32px;
    z-index: 10;
  }
  .content-r img{
    left: -20px;
  }
  .time-line::after{
    content: '';
    position: absolute;
    width: 6px;
    height: 100%;
    background: #1e90ff;
    border-radius: 10px;
    top: 0;
    left: 50%;
    margin-left: -3px;
    z-index: -1;
  }
  .tex-box h2{
    font-weight: 600;
  }
  .tex-box p{
    display: inline-block;
    margin-bottom: 15px;
  }
  .left-content-arrow{
    height: 0;
    width: 0;
    top: 28px;
    position: absolute;
    z-index: 1;
    border-top: 15px solid transparent;
    border-bottom: 15px solid transparent;
    border-left: 15px solid #000;
    right: -15px;
  }
  .right-content-arrow{
    height: 0;
    width: 0;
    top: 28px;
    position: absolute;
    z-index: 1;
    border-top: 15px solid transparent;
    border-bottom: 15px solid transparent;
    border-right: 15px solid #000;
    left: -15px;
  }


  /*  Contact Section */
  .contact-section{
    width: 80%;
    margin: 50px auto;
    background-color: #fff;
  }
.contact-box{
  background: #fff;
 
}
.contact-left{
  flex-basis: 60%;
  padding: 40px 60px;
}
.contact-right{
    height: 80vh;
  flex-basis: 40%;
  padding: 40px;
  background: #2294ed;
  color: #fff;
}
.input-row{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-bottom: 20px;
  }
  .input-row .input-group
  {
    flex-basis: 45%;
  }
  input{
    width: 100%;
  }
  input{
    border: none;
    width: 100%;
    border-bottom: 1px solid #ccc;
    outline: none;
    padding: 6px;
  }
  textarea{
    width: 100%;
    border: 1px solid #ccc;
    outline: none;
    padding: 10px;
    box-sizing: border-box;
  }
  label{
    margin-bottom: 6px;
    display: block;
    color: var(--secondary-text-color);
  }
  button{
    background-color: #2294ed;
    width: 100px;
    border: none;
    outline: none;
    color: #fff;
    cursor: pointer;
    height: 35px;
    border-radius: 30px;
    margin-top: 20px;
    box-shadow: 0px 5px 15px 0px rgb(28, 0, 181, 0.3);
  }
  .contact-left h3{
    color: #2294ed;
    font-weight: 600;
    margin-bottom: 30px;
  }
  .contact-right h3{
   
    font-weight: 600;
    margin-bottom: 30px;
  }
  tr td:first-child{
    padding-right: 20px;
  }
  tr td{
    padding-top: 20px;
  }

  /*Footer */
.footer-container{
    width: 100%;
    height: 420px;
    padding: 80px 20px;
    display: flex;
   
    justify-content: space-around;
    background-color: #183b54;
  }
  
  .name h2{
    color: #fff;
  }
  .cnt a{
    text-decoration: none;
    color: #fff;
    padding: 10px 14px;
    font-weight: 400;
    font-size: 20px;
  }
  .icons a{
    text-decoration: none;
    color: #fff;
    padding: 10px 14px;
    font-weight: 400;
    font-size: 22px;
  }
   /* Subfooter*/
   .sub-footer{
      background-color: #b9acde;
      
   }
   .subfooter-container{
    display: flex;
    height: 60px;
    align-items: center;
    justify-content: center;
    gap: 30px;
  }
  .subfooter-container a{
      text-decoration: none;
      color: #183b56;
      font-size: 20px;
      font-weight: 700;
  }
</style>
<body>
    <!--HOME-->
    <section id="home">
        <!--Nav - Bar-->
    <nav>
        <div class="container flex main-nav">
            <div class="logo">
                Portfolio
            </div>
            <div class="nav-links">
                <ul class="flex">
                    <li><a href="#" class="hover-link active">Home</a></li>
                    <li><a href="#About" class="hover-link" >About</a></li>
                    <li><a href="#projects" class="hover-link">Skills</a></li>
                    <li><a href="#Skills" class="hover-link">Projects</a></li>
                    <li><a href="#education" class="hover-link">Education</a></li>
                    <li><a href="#contact" class="hover-link secondary-btn">Contact me</a></li>
                </ul>
            </div>
            <a href="#" class="nav-toggle hover-link"><i class="fa-solid fa-bars"></i></a>
        </div>
    </nav>
    <!--Header-->
    <header>
        <div class="container header-section flex">
            <div class="headre-left">
                <h2>Hey ! My name is</h3>
                <h2> <span>Harsh Vardhan</span> </h2>
                <p>I am a passionate</p> 
               <p><span id="element"></span></p>
               <a href="#" class="primary-btn get-strated">Get Strated</a>
            </div>
            <div class="header-right">
                <img src="developer.png" alt="">
            </div>
        </div>
    </header>
</section>
<br><br>
<!-- About Section -->
<section id="About">
    <div class="container headings ">
        <h1>Amout Me</h1>
        <h2>My Introduction </h2>
    </div>
    <div class="about-section container flex">
    <div class="about-left">
       <img src="image.jpg" alt="">
    </div>
    <div class="about-right">
        <p>Hey 👋 , I'm a 19-year-old undergraduate pursuing a degree in Computer Science and Engineering, with a passion for software development. As an aspiring Full-Stack Web Developer, I'm eager to gain hands-on experience and learn from industry professionals by securing internships in the field. I'm excited to contribute my skills to innovative projects and work collaboratively with teams to bring ideas to life. Through internships, I hope to gain real-world experience and learn from experienced mentors while also developing my skills in software development.
        </p>
     </div>
    </div>
    <div class="btn flex container">
        <button class="primary-btn cv">Download My, CV</button>
    </div>
</section>
<br><br>
<!--Projects-->
<section id="projects">
    <section id="project">
        <div class="container headings ">
            <h1>Projects</h1>
            <h2>See My Projects </h2>
        </div>
        
        <div class="gallery-wrap">
            <img src="back.png" id="backbtn">
            <div class="gallery">
                  <div>
                   <span><img src="snake.jpg" alt=""></span>
                   </div>
                   <div>
                    <span><img src="calculator.jpg" alt=""></span>
                   </div>
                   <div>
                    <span><img src="dg.jpg" alt=""></span>
                    </div>
                    <div>
                    <span><img src="tm.jpg" alt=""></span>
                   </div>
                   <span><img src="images/image-5.png" alt=""></span>
                   <span><img src="images/image-6.png" alt=""></span>
               </div>
            <img src="next.png" id="nextbtn">
       </div>
    </section>    
</section>
<br><br>
<!--Skills-->
<section id="Skills">
    <div class="container headings ">
        <h1>My Skills
        </h1>
        <h2>My Technical Skills
        </h2>
    </div>
    <div class="skills-section container flex">
        <div class="skills-area flex">
            <div class="skills-card flex"><img src="html.png" alt=""></div>
            <div  class="skills-card flex"><img src="css.png" alt=""></div>
            <div  class="skills-card flex"><img src="js.jpg" alt=""></div>
            <div  class="skills-card flex"><img src="bootstrap.jpg" alt=""></div>
            <div  class="skills-card flex"><img src="node.png" alt=""></div>
            <div  class="skills-card flex"><img src="c++.png" alt=""></div>
            <div  class="skills-card flex"><img src="pyhton.png" alt=""></div>
            <div  class="skills-card flex"><img src="java.png" alt=""></div>
            
        </div>
    </div>
</section>

<br><br>

<section id="education">
    <div class="container headings ">
        <h1>Education
        </h1>
        <h2>My Educational Qualifications
        </h2>
    </div>
    <div class="education-content">
        <div class="time-line">
            <div class="content-p content-l">
                <img src="logo-i.png" alt="">
                <div class="tex-box">
                   
                    <div class="education-1">
                        <h3 class="h3">B.Tech Computer Science and Engineering</h3>
                        <p class="p-i">Institute of Engineering and Technology, Udaipur (IET, MLSU)</p>
                        <h4  class="p-i"><i class="fa-regular fa-calendar"></i>    Aug-2022 - Jun-2026</h4>
                        <span class="left-content-arrow">
    
                        </span>
                    </div>
                </div>
            </div>
            <div class="content-p content-r">
                <img src="logo-i.png" alt="">
               
                <div class="tex-box">
        
                    <div class="education-2">
                        <h3 class="h3">Senior Secondary School</h3>
                       <p class="p-i">Rashtra Bharti Academy Sr. Sec. School Udaipur</p>
                       <h4 class="p-i"><i class="fa-regular fa-calendar"></i>  Jul-2022 - Apr-2022</h4>
                   </div>
                   <span class="right-content-arrow">
                            
                </span>
                </div>
            </div>
            <div class="content-p content-l">
                <img src="logo-i.png" alt="">
               
                <div class="tex-box">
                  
                    <div class="education-3"> 
                        <h3 class="h3">Secondary School</h3>
                        <p  class="p-i">Rashtra Bharti Academy Sr. Sec. School Udaipur</p>
                        <h4  class="p-i"><i class="fa-regular fa-calendar"></i>    Aug-2007 - Apr-2020</h4>
                    </div>
                    <span class="left-content-arrow">           
                        </span>
                </div>
            </div>
         </div>
         </div>
</section>

<!-- Contact Section -->
<section id="contact">
    <div class="container headings ">
        <h1>Contact Us
        </h1>
        <h2>Feel Free To Contact with us
        </h2>
    </div>
        <div class="contact-section flex container">
            <div class="contact-left">
               <h3>Sent Your Request</h3>
               <form>
                <div class="input-row">
                    <div class="input-group">
                        <label>NAME</label>
                        <input type="text" placeholder="Your name">
                    </div>
                    <div class="input-group">
                        <label>PHONE</label>
                        <input type="text" placeholder="+91 412 520 685">
                    </div>
                    <div class="input-group">
                        <label>E-Mail</label>
                        <input type="email" placeholder="E-Mail">
                    </div>
                    <div class="input-group">
                        <label>Subject</label>
                        <input type="text" placeholder="Product Demo">
                    </div>
                </div>
                <label>Message</label>
                <textarea rows="5" placeholder="Your Message"></textarea>
               </form>
               <button type="submit">Send</button>
            </div>
            <div class="contact-right">
             <h3>Reach Us</h3>
             <table>
                <tr>
                    <td>Email</td>
                    <td>contactus@example.com</td>
                </tr>
                <tr>
                    <td>Phone</td>
                    <td>+91 0123655</td>
                </tr>
                <tr>
                    <td>Adress</td>
                    <td>#212  grown flow, 7th cross <br>
                    Some Layout, Some Road</td>
                </tr>
             </table>
            </div>
        </div>
</section>

<!--Footer-->
    
<footer>
    <div class="footer-container">
       
            <div class="name">
                <h2>Harsh Vardhan</h2>
                <h2>Full-Stack Web-Developer</h2>
            </div>
            <div class="cnt">
                <a href="#">About</a>
                <a href="#">Projects</a>
                <a href="#">Contact</a>
            </div>
            <div class="icons">
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-github"></i></a>
            </div>
        </div>
    
</footer>

<!--Sub Footer-->

<div class="sub-footer">
    <div class="subfooter-container">
    <a href="#"><i class="fa-brands fa-twitter"></i></a>
    <a href="#"><i class="fa-brands fa-facebook"></i></a>
    <a href="#"><i class="fa-brands fa-linkedin"></i></a>
    </div>
</div>
<script src="js.js"></script>
    <script src="https://unpkg.com/typed.js@2.0.16/dist/typed.umd.js"></script>
 <script>
    var typed = new Typed('#element', {
      strings: ['Full-Stack Web Developer', 'Graphic Designer', 'Machine Learning'],
      typeSpeed: 50,
    });
    let scrollContainer = document.querySelector(".gallery");
let backbtn = document.getElementById("backbtn");
let nextbtn = document.getElementById("nextbtn");

scrollContainer.addEventListener("wheel", (evt)=>{
    evt.preventDefault();
    scrollContainer.scrollLeft += evt.deltaY;
    scrollContainer.style.scrollBehavior = "auto";
});
nextbtn.addEventListener("click", ()=>{
    scrollContainer.style.scrollBehavior = "smooth";
    scrollContainer.scrollLeft += 900;
});
backbtn.addEventListener("click", ()=>{
    scrollContainer.style.scrollBehavior = "smooth";
    scrollContainer.scrollLeft -= 900;
});
  </script>
 


</body>
</html>
