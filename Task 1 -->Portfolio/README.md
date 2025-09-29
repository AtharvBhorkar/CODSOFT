<!DOCTYPE html>
<html>

<head>
    <title>Atharv</title>

    <style>
        * { 
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            height: 2800px ;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: rgb(3, 24, 41);
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            overflow-x: hidden;

        }

        #topbar {
            position: absolute;
            top: 20px;
            right: 40px;
            display: flex;
            gap: 25px;
            opacity: 0.5;
        }

        #topbar a {
            color: white;
            text-decoration: none;
            font-weight: 500;
        }

        #topbar a:hover {
            color: #01457b;
        }
        #line {
            position: absolute;
            top: 60px;
            background: white;
            width: 100%;
            opacity: 0.1;
        }
        .logo-badge{
            position: absolute;
            width: 40px;
            height: 40px;
            left: 10%; 
            top: 15px;
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            font-size: 21px;
            background: linear-gradient(135deg, #00c3ff, #0066ff);
            display: grid;
            place-items: center;
            color: white;
            border-radius: 10px;
        }
        .logo-text{
            position: absolute;
            left: 13.2%; 
            top: 23px;
            font-family:serif;
            font-size: 21px;
            display: grid;
            place-items: center;
            color: white;
            border-radius: 10px;
            
        }

        .Description{
           position: absolute;
           top: 160px;
           width: 1200px;
           height: 450px;
           background-color: #001e39;
           border: 1px solid rgb(30, 63, 63);
           backdrop-filter: blur(10px);
           box-shadow: 0 0 10px #051527;
           color: white;
           border-radius: 10px;
           padding: 30px 40px;
           box-shadow: 0 1px 8px blue;
        }

        .Description h1{
            font-size: 70px;
            font-weight: 200;
            font-family:'Times New Roman', Times, serif;
        }

        .Description h5{
            font-size: 21px;
            font-weight: bolder;
        }

        .Description pre{
            font-size: 17px;
            opacity: 0.6;
        }

        button{
            position: absolute;
            top: 50px;
            left: 200px;
            color: whitesmoke;
            font-weight: bold;
            margin-top:460px;
            height: 55px;
            width: 165px;
            background: linear-gradient(135deg, #00c3ff, #0066ff);
            border: 1px solid #0066ff;
            border-radius: 40px;
            font-size: 18px;
            box-shadow: 5px 10px 30px #0f4a80;
        }
        
        button:hover:active{
            background: linear-gradient(45deg, #062442);
            color:  #1270c2;
        }

        .abt{
            position: absolute;
            top: 760px;
            left: 169px;
            font-weight: 900;
            color: whitesmoke;
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            font-size: 25px;
        }
        .abt img{
            position: absolute;
            top: 70px;
            left: 5px;
            height: 280px;
            width: 230px;
            border-radius: 20%;
        }
        .abt pre{
            position: absolute;
            top: 110px;
            left: 290px;
            font-size: 18px;
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            font-weight: 100;
            opacity: 0.7;
        }
        .abt p{
            color: white;
            position: absolute;
            width: 350px;
            top: 270px;
            left: 290px;
            font-size: 18px;
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            font-weight: 100;
            opacity: 0.8;

        }
        .facts{
           position: absolute;
           right: 10px;
           top: 890px;
           width: 610px;
           height: 170px;
           background-color: #001e39;
           border: 1px solid rgb(30, 63, 63);
           backdrop-filter: blur(10px);
           box-shadow: 0 0 10px #051527;
           color: white;
           border-radius: 10px;
           padding: 20px 30px;
           box-shadow: 0 2px 10px blue;
        }
        .facts span{
            font-size: 20px;
            font-weight: bolder;
        }
        .facts pre{
            font-size: 15px;
            padding: 0px 40px;
            opacity: 0.8;
        }
        
        .skills {
            position: absolute;
            top: 320px;
            right: 560px;
            font-weight: 900;
            color: white;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            font-size: 17px;
        }

        .skill-list {
            list-style: none;
            margin: 20px;
            display: flex;
            gap: 20px;
        }

        .skill-list li {
            background: transparent;
            color: white;
            padding: 10px 30px;
            border: 2px solid #0b355b;
            border-radius: 8px;
            font-size: 18px;
            font-weight: 500;
        }
        .projects h2{
            position: relative;
            top: 350px;
            right: 753px;
            font-size: 26px;
            font-weight: bolder;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
        }
        .projects img{
            position: relative;
            top: 420px;
            right: 750px;
            height: 190px;
            width: 300px;
            border-top-left-radius: 30px;
            border-top-right-radius: 30px;
            border: 1px solid silver;
        }
        .projects .name{
            position: relative;
            top: 431px;
            right: 748px;
            font-size: 17px;
            font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }
        .projects p{
            position: relative;
            top: 445px;
            right: 750px;
            width: 320px;
            opacity: 0.8;
        }
        .projects a{
            position: relative;
            top: 450px;
            right: 749px;
            font-size: 20px;
            color: #4a92c9;
            text-decoration: none;
            font-family:'Times New Roman', Times, serif

        }
        .project2 img{
            position: relative;
            top: 125px;
            right: 320px;
            height: 190px;
            width: 300px;
            border-top-left-radius: 30px;
            border-top-right-radius: 30px;
            border: 1px solid silver;
        }
        .project2 .name{
            position: relative;
            top: 137px;
            right: 320px;
            font-size: 17px;
            font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }
        .project2 p{
            position: relative;
            top: 145px;
            right: 320px;
            width: 320px;
            opacity: 0.8;
        }
        .project2 a{
            position: relative;
            top: 155px;
            right: 321px;
            font-size: 20px;
            color: #4a92c9;
            text-decoration: none;
            font-family:'Times New Roman', Times, serif
        }
        
        .project3 img{
            position: relative;
            bottom: 171px;
            left: 110px;
            height: 190px;
            width: 300px;
            border-top-left-radius: 30px;
            border-top-right-radius: 30px;
            border: 1px solid silver;
        }
        .project3 .name{
            position: relative;
            bottom: 160px;
            left: 110px;
            font-size: 17px;
            font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }
        .project3 p{
            position: relative;
            bottom: 151px;
            left: 110px;
            width: 320px;
            opacity: 0.8;
        }
       .project3 a{
            position: relative;
            bottom: 140px;
            left: 112px;
            font-size: 20px;
            color: #4a92c9;
            text-decoration: none;
            font-family:'Times New Roman', Times, serif
        }

        .resume h2{
            position: relative;
            bottom: 30px;
            right: 750px;
            font-size: 26px;
            font-weight: bolder;
            font-family: Verdana, Geneva, Tahoma, sans-serif;        
        }

        .resume p{
            position: relative;
            bottom: 15px;
            right: 748px;
            opacity: 0.9;
        }
        .resume a{
            position: relative;
            top: 23px;
            right: 748px;
            height: 10px;
            padding: 15px 50px;
            width: 150px;
            font-weight: lighter;
            border: 2px dotted rgb(91, 90, 90);
            border-radius: 10px;
            font-size: 15px;
            color: #0066ff;
            text-decoration: none;
        }
        .contact h2{
            position: relative;
            top: 110px;
            right: 749px;
            font-size: 26px;
            font-weight: bolder;
            font-family: Verdana, Geneva, Tahoma, sans-serif;            
        }

        .contact-details{
           position: absolute;
           top: 1400px;
           right: 755px;
           width: 570px;
           height: 280px;
           background-color: #001e39;
           border: 1px solid rgb(30, 63, 63);
           backdrop-filter: blur(10px);
           box-shadow: 0 0 10px #051527;
           color: white;
           border-radius: 10px;
           padding: 30px 40px;
        }

        .contact-details p{
            font-size: 15px;
            font-family: Verdana, Geneva, Tahoma, sans-serif;            
        }
        .contact-details span{
            position: relative;
            top: 25px;
            font-size: 16px;
            font-weight: lighter;
            font-family: Verdana, Geneva, Tahoma, sans-serif;  
            opacity: 0.7;          
        }
        .contact-fill{
           position: absolute;
           top: 1400px;
           right: 155px;
           width: 570px;
           height: 380px;
           background-color: #001e39;
           border: 1px solid rgb(30, 63, 63);
           backdrop-filter: blur(10px);
           box-shadow: 0 0 10px #051527;
           color: white;
           border-radius: 10px;
           padding: 30px 40px;
        }
        .contact-fill input{
            text-align: left;
            height: 50px;
            width: 450px;
            font-size: 15px;
            border-radius: 20px;
            color: rgb(222, 221, 221);
            background-color:#011e39;
            border: 2px solid rgb(82, 80, 80);
        }
        .contact-fill textarea{
            position: relative;
            top: 20px;
            height: 100px;
            width: 450px;
            font-size: 15px;
            color: rgb(222, 221, 221);
            border-radius: 20px;
            background-color:   #011e39;
            border: 2px solid rgb(82, 80, 80);
        }
        .contact-fill button{
            margin-top: 252px;
            margin-left: -160px;
            height: 45px;
            width: 450px;
            color: whitesmoke;
            font-weight: bold;
        }
        footer{
            position:relative;
            top:680px; 
            text-align:center;
            color:white;
            opacity:0.6; 
            font-size:14px;
        }
    </style>
</head>
<body>
    <div class="logo">
            <span class="logo-badge">AB</span>
            <span class="logo-text">Atharv Bhorkar</span>
    </div>
    <div id="fullpage">
        <div id="topbar">
            <a href="#">HOME</a>
            <a href="#skills">SKILLS</a>
            <a href="#about">ABOUT ME</a>
            <a href="#projec">PROJECTS</a>
            <a href="#contactt">CONTACT</a>
        </div>

        
        </div>
    <hr id="line">
    <div class="Description">
            <h1>Hello, It's Me</h1>
            <h1>Atharv Bhorkar</h1>
            <h5>And I'm a <span style="font-size: 30px; color: #1c83dd;">Frontend Developer</span></h5>
            <pre>

I focus on crafting clean and interactive websites. I believe that every
line of code should add value to the user’s experience and make the digital 
journey seamless.
            </pre>
        </div>
        <a href=""><button>View Projects →</button></a>

    <section class="abt" id="about">
        <span>About</span>
        <img src="https://i.ibb.co/Y4Dd5X8v/Whats-App-Image-2025-09-04-at-00-11-06-2ad777a9.jpg" alt="">
        <pre>
"Hi, I'm Atharv — a frontend developer who
loves turning ideas into delightful web 
experiences. I focus on semantic HTML, 
scalable CSS, and intuitive interactions, 
and I learn best by building."
        </pre>
        <p>Location: India • Open to freelance & internships</p>
    </section>
        
    <section class="facts">
        <span>Quick facts:</span>
        <pre>

<li>💡 Strong in HTML/CSS, improving in JS</li>
<li>⚙️ Comfortable with Git & GitHub basics</li>
<li>🎯 Goal: Build responsive, accessible UIs</li>
        </pre>
    

    <section class="skills" id="skills">
    <h2>Skills</h2>
    <ul class="skill-list">
        <li>HTML5</li>
        <li>CSS3</li>
        <li>JavaScript (Learning)</li>
        <li>React (Learning)</li>
        <li>Java</li>
    </ul>
    </section>


    <div class="projects" id="projec">
        <h2>Projects</h2>
        <img src="https://i.ibb.co/rNwQ3g9/Screenshot-2025-09-04-221457.png" alt="">
        <h2 class="name">Login Page UI</h2>
        <p>Glassmorphism inspired login form with hover effects and gradient background. Designed with pure HTML & CSS.</p>
        <a href="login-page.html">view↗</a>
    </div>

    <div class="project2">
        <img src="https://i.ibb.co/JwKBcDBj/Screenshot-2025-09-06-142302.png" alt="">
        <h2 class="name">LinkedIn Page UI</h2>
        <p>LinkedIn homepage clone with login and signup UI, built using pure HTML & CSS to practice real-world layout design.</p>
        <a href="LinkdinPage1.html">view↗</a>
    </div>

    <div class="project3">
        <img src="https://i.ibb.co/ZzJVz6th/Screenshot-2025-09-06-143848.png" alt="">
        <h2 class="name">MCPS Noida Page</h2>
        <p>Dedicated blog page for MCPS Noida to share latest updates, educational tips, and event highlights.</p>
        <a href="Spproj.html">view↗</a>
    </div>

    <div class="resume">
        <h2>Resume</h2>
        <p>View my resume in PDF format</p>
        <a href="https://i.ibb.co/vxcwX8JX/Atharv-resume.jpg">View Resume (PDF)</a>
    </div>

    <div class="contact" id="contactt">
        <h2>Contact</h2>
    </div>
    <section class="contact-details">
        <p>Email: <a href="mailto:atharvbhorkar19@gmail.com">atharvbhorkar19@gmail.com</a></p>
        <br>
        <p>Phone: <a href="tel:+919604224586">+91 96042 24586</a></p>
        <span>Feel free to reach out for collaborations or just a friendly hello 👋</span>
    </section>

    <section class="contact-fill">
        <form>
        <input type="text" placeholder="Your Name" required> 
        <br>
        <br>
        <input type="text" placeholder="Enter Email" required>
        <textarea placeholder="Enter Message" required></textarea>
        <button type="submit">Send Message</button>
        </form>
    </section>
    <footer>
        © 2025 Atharv Bhorkar | All Rights Reserved
    </footer>

       
</body>

</html>




