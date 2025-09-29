<!DOCTYPE html>
<html lang="en">

<head>

    <title>Landing Page</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500&family=Roboto:wght@400&display=swap"
        rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            height: 2600px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            overflow-x: hidden;
        }

        .video-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.8;
        }

        .logo-badge {
            position: fixed;
            width: 48px;
            height: 40px;
            left: 10%;
            top: 15px;
            font-family: "Love Ya Like A Sister", cursive;
            font-size: 21px;
            background: linear-gradient(135deg, #00c3ff, #0066ff);
            display: grid;
            place-items: center;
            color: white;
            border-radius: 10px;
            cursor: pointer;
        }

        .logo-nam {
            position: fixed;
            left: 13.2%;
            font-family: "Love Ya Like A Sister", cursive;
            top: 23px;
            font-size: 21px;
            display: grid;
            place-items: center;
            color: white;
            border-radius: 10px;
            cursor: pointer;
        }

        .top {
            position: fixed;
            bottom: 730px;
            right: 90px;
            display: flex;
            gap: 70px;
        }

        .top a {
            color: white;
            text-decoration: none;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }
        .top a:hover{
            color: rgb(45, 38, 38);
        }

        .top-bar {
            position: fixed;
            bottom: 700px;
            top: 0;
            height: 80px;
            width: 1550px;
            background-color: rgba(0, 0, 0, 0.9);
        }

        .details {
            position: absolute;
            top: 120px;
            background-color: rgba(0, 0, 0, 0.5);
            height: 700px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-radius: 20px;
        }

        .details h1 {
            position: relative;
            bottom: 150px;
            left: 125px;
            color: white;
            font-size: 60px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        .details p {
            position: relative;
            bottom: 75px;
            right: 200px;
            color: white;
            font-size: 35px;
            font-weight: bolder;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
            text-shadow: 0px 0px 50px rgb(84, 81, 80);
            color: rgba(255, 174, 0, 0.2);
        }

        .details button {
            position: relative;
            top: 0px;
            right: 330px;
            height: 50px;
            width: 150px;
            color: white;
            font-size: 20px;
            border-bottom-right-radius: 20px;
            border-bottom-left-radius: 20px;
            border: none;
            background-color: rgba(125, 239, 11);
            font-weight: bolder;
            cursor: pointer;
        }

        .details button:hover {
            background-color: rgba(247, 243, 243, 0.1);
            color: white;
            border: 1px dotted rgba(69, 28, 28, 0.5);
        }

        .about {
            position: absolute;
            top: 850px;
            background-color: rgba(0, 0, 0, 0.5);
            height: 300px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-radius: 20px;
        }

        .about h1 {
            position: relative;
            bottom: 90px;
            left: 430px;
            color: white;
            font-size: 40px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        .about p {
            position: relative;
            top: 0px;
            right: 40px;
            color: rgb(220, 182, 182);
            font-size: 20px;
            font-weight: lighter;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }

        .our-programs {
            position: absolute;
            top: 1200px;
            background-color: rgba(0, 0, 0, 0.5);
            height: 300px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-radius: 20px;
        }

        .our-programs h1 {
            position: relative;
            bottom: 100px;
            left: 630px;
            color: white;
            font-size: 36px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

        }

        .our-programs #card {
            position: relative;
            right: 70px;
            height: 70px;
            width: 200px;
            padding: 25px 20px;
            color: white;
            font-size: 17px;
            background: rgba(255, 255, 255, 0.1);
            margin: 55px;
            border-radius: 20px;
            text-align: center;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }

        #card:hover {
            background-color: rgba(138, 62, 62, 0.1);
        }

        .our-trainers {
            position: absolute;
            top: 1550px;
            background-color: rgba(0, 0, 0, 0.5);
            height: 500px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-radius: 20px;
        }

        .our-trainers h1 {
            position: relative;
            bottom: 210px;
            left: 330px;
            color: white;
            font-size: 38px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }
        .our-trainers :hover {
            background-color: rgba(255, 0, 0, 0.2);
            box-shadow: 10px 10px 30px rgb(151, 98, 98);
        }

        .trainer-card1 img {
            position: relative;
            height: 200px;
            border-radius: 90%;
        }

        .trainer-card1 {
            position: relative;
            top: 35px;
            right: 400px;
            height: 350px;
            width: 220px;
            background-color: rgba(255, 255, 255, 0.2);
            padding: 18px;
        }

        .trainer-card1 button {
            position: relative;
            height: 40px;
            width: 110px;
            background-color: red;
            top: 15px;
            border-radius: 20px;
            border: none;
            cursor: pointer;
        }

        .trainer-card2 img {
            position: relative;
            height: 200px;
            border-radius: 90%;
        }

        .trainer-card2 {
            position: relative;
            top: 35px;
            right: 100px;
            height: 350px;
            width: 220px;
            background-color: rgba(255, 255, 255, 0.2);
            padding: 18px;
        }

        .trainer-card2 button {
            position: relative;
            height: 40px;
            width: 110px;
            background-color: red;
            top: 15px;
            border-radius: 20px;
            border: none;
            cursor: pointer;
        }

        .trainer-card3 img {
            position: relative;
            height: 200px;
            border-radius: 90%;
        }

        .trainer-card3 {
            position: relative;
            top: 35px;
            left: 180px;
            height: 350px;
            width: 220px;
            background-color: rgba(255, 255, 255, 0.2);
            padding: 18px;
        }

        .trainer-card3 button {
            position: relative;
            height: 40px;
            width: 110px;
            background-color: red;
            top: 15px;
            border-radius: 20px;
            border: none;
            cursor:pointer;
        }

        .contact-us {
            position: absolute;
            top: 2100px;
            background-color: rgba(0, 0, 0, 0.5);
            height: 500px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-radius: 20px;
        }

        .contact-us h1 {
            position: relative;
            bottom: 205px;
            left: 178px;
            color: white;
            font-size: 36px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            align-items: center;
        }

        form input,
        form textarea,
        form button {
            position: relative;
            right: 75px;
            width: 350px;
            max-width: 400px;
            padding: 10px;
            border-radius: 10px;
            border: 1px solid #ccc;
            outline: none;
        }

        form button {
            background-color: rgba(125, 239, 11);
            cursor: pointer;
        }

        form button:hover {
            background-color: rgba(247, 243, 243, 0.1);
            color: white;
            border: 1px dotted rgba(69, 28, 28, 0.5);
        }

        
    </style>
</head>

<body>
    <section class="top-bar">
        <video autoplay muted loop class="video-bg">
            <source src="thebgvideo.mp4" type="video/mp4">
            Your browser does not support HTML5 video.
        </video>
        <header>
            <nav>
                <span class="logo-badge">AB's</span>
                <span class="logo-nam">Landing Page</span>
                <div class="top">
                    <a href="#home">HOME</a>
                    <a href="#about">ABOUT</a>
                    <a href="#prog">PROGRAMS</a>
                    <a href="#train">TRAINERS</a>
                    <a href="#cont">CONTACT</a>
                </div>
            </nav>
        </header>
    </section>
    <section class="details" id="home">
        <h1>Transform Your Body</h1>
        <p>With us</p>
        <button>Join Now</button>
    </section>
    <section class="about" id="about">
        <h1>About us</h1>
        <p>We are dedicated to helping you reach your fitness goals with professional trainers and modern equipment.</p>
    </section>
    <section class="our-programs" id="prog">
        <h1>Our Programs</h1>
        <div id="card">Strength Training</div>
        <div id="card">Yoga Classes</div>
        <div id="card">Cardio Sessions</div>
        <div id="card">Calisthenics Traininig</div>
    </section>
    <section class="our-trainers" id="train">
        <h1>Our Trainers</h1>
        <div class="trainer-card1">
            <img src="https://i.ibb.co/ZRPxy5jm/images.jpg" alt="Trainer">
            <h2>Rahul Sharma</h2>
            <p>Certified Fitness Trainer<br>Strength & Conditioning</p>
            <button>View Profile</button>
        </div>
        <div class="trainer-card2">
            <img src="https://i.ibb.co/04fXQv7/yoga.jpg" alt="Yoga Trainer">
            <h2>Anjali Verma</h2>
            <p>Certified Yoga Instructor<br>Mind & Body Wellness</p>
            <button>View Profile</button>
        </div>

        <div class="trainer-card3">
            <img src="https://i.ibb.co/ZzhgZwhY/calisthe.jpg" alt="Calisthenics Trainer">
            <h2>Arjun Mehta</h2>
            <p>Certified Calisthenics Coach<br>Bodyweight Training Expert</p>
            <button>View Profile</button>
        </div>
    </section>
    <section class="contact-us" id="cont">
        <h1>Contact Us</h1>
        <form>
            <input type="text" placeholder="Your Name">
            <input type="text" placeholder="Your Email">
            <textarea rows="4" placeholder="Your Message"></textarea>
            <button>Send</button>
        </form>
    </section>
</body>

</html>
