# Ex01 Portfolio
## Date: 12-03-2024

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header Section -->
    <header class="header">
        <a href="#" class="logo"><span>Saranya S</span> <br> B.Tech IT 2nd Year<br> </a>
        <nav class="navbar">
            <a href="#home" class="activate">HOME</a>
            <a href="#experience">EXPERIENCE</a>
            <a href="#about">ABOUT</a>
            <a href="#contact">CONTACT</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="home">
        <div class="home-container">
            <div class="home-content">
                <h3>Hi!</h3>
                <h1>I'm <span>Saranya S</span>, a Frontend Developer</h1>
                <p>Passionate about creating interactive and responsive websites using HTML, CSS, and JavaScript.</p>
            </div>
            <div class="home-image">
                <img src="img.jpg" alt="Saranya S">
            </div>
        </div>
    </section>
    

    <section id="experience" class="experience">
        <h2>Experience</h2>
    
        <!-- Project Experience -->
        <div class="experience-item">
            <h3>Project: Farmer-to-Buyer App</h3>
            <p>A mobile app that connects farmers directly with buyers, eliminating intermediaries.</p>
            <p><strong>Tech Stack:</strong> HTML, CSS, JavaScript, React Native</p>
        </div>
    
        <!-- Resume Section -->
        <div class="experience-item">
            <h3>My Resume</h3>
            <p>
                I am a <strong>B.Tech Information Technology</strong> student at <strong>Saveetha Engineering College</strong>, expected to graduate in <strong>May 2027</strong>.  
                I am passionate about frontend development, with expertise in HTML, CSS, JavaScript, and React.  
            </p>
            <p>
                <strong>Technical Skills:</strong>  
                - Web Technologies: HTML, CSS, JavaScript, React  
                - Backend: Node.js, Express  
                - Database: MySQL, MongoDB  
                - Tools: Git, GitHub, VS Code  
            </p>
            <p>
                <strong>Certifications:</strong>  
                - Frontend Development Internship at CodeAlpha (Feb 2025)  
                - Responsive Web Design Certification from FreeCodeCamp  
            </p>
            <p>
                <strong>Achievements:</strong>  
                - Developed a Farmer-to-Buyer App to eliminate middlemen in agriculture trade.  
                - Participated in Smart India Hackathon 2025** with an innovative web project.  
            </p>
        </div>
    </section>
    
    

<!-- About Section -->
<section id="about" class="about">
    <h2>About Me</h2>
    <div class="about-box">
        <p>
            I am currently a <strong>B.Tech Information Technology student</strong> at <strong>Saveetha Engineering College</strong>, expected to graduate in <strong>May 2027</strong>.  
            Passionate about <strong>frontend development</strong>, I enjoy designing user-friendly interfaces using <strong>HTML, CSS, JavaScript, and React</strong>.
        </p>
    </div>
</section>

<!-- Contact Section -->
<section id="contact" class="contact">
    <h2>Contact Me</h2>
    <div class="contact-box">
        <p><strong>Email:</strong> saranyaselvam@gmail.com</p>
        <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/saranya-s-b275a32a0" target="_blank">www.linkedin.com/in/saranya-s</a></p>
        <p><strong>GitHub:</strong> <a href="https://github.com/ssaranya27" target="_blank">github.com/ssaranya27</a></p>
        <p><strong>Phone:</strong> +91 6579372340</p>
    </div>
</section>

</body>
</html>
```
Style.css
```

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins', sans-serif;
    text-decoration: none;
    list-style: none;
}

.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 35px 12%;
    background: rgb(173, 109, 109);
    backdrop-filter: blur(10px);
    display: flex;
    justify-content: space-between;
    z-index: 100;
}

.logo {
    font-size: 25px;
    color: white;
    font-weight: 600;
    transition: 0.3s ease;
}

.logo:hover {
    color: orchid;
    text-shadow: 0 0 25px orchid;
    transform: scale(1.1);
}

span {
    color: orchid;
}

.navbar a {
    font-size: 18px;
    color: white;
    font-weight: 500;
    margin: 0 20px;
    border-bottom: 3px solid transparent;
    transition: 0.3s ease;
}

.navbar a:hover,
.navbar a.activate {
    color: orchid;
    border-bottom: 3px solid orchid;
}

.home {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: #f5f5f5;
    padding: 50px 12%;
}

.home-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
}

.home-content {
    max-width: 50%;
}

.home-image img {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    object-fit: cover;
    border: 5px solid orchid;
    box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.2);
}

.contact {
    width: 100%;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: #e6e6e6;
    padding: 50px 12%;
}

.contact h2 {
    font-size: 32px;
    color: #333;
    margin-bottom: 20px;
}

.contact-box {
    background: white;
    padding: 40px;
    max-width: 900px;
    width: 100%;
    text-align: center;
    border-radius: 10px;
    box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.2);
    border-left: 6px solid orchid;
}

.contact-box p {
    font-size: 18px;
    line-height: 1.8;
    color: #333;
    margin: 10px 0;
}

.contact-box a {
    color: #ff6600;
    text-decoration: none;
    font-weight: bold;
}

.contact-box a:hover {
    text-decoration: underline;
}

.experience-item {
    background: #d08080;
    padding: 20px;
    border-radius: 10px;
    margin: 20px auto;
    width: 70%;
    text-align: left;
    box-shadow: 5px 5px 15px rgba(239, 234, 234, 0.2);
}

.experience-item h3 {
    color: #f8f2ee;
}

.experience-item p {
    font-size: 16px;
    line-height: 1.6;
}

.about {
    width: 100%;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #f5f5f5;
    padding: 50px 12%;
}

.about-box {
    background: white;
    padding: 40px;
    max-width: 900px;
    width: 100%;
    text-align: center;
    border-radius: 10px;
    box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.2);
    border-left: 6px solid orchid;
}

.about-box p {
    font-size: 18px;
    line-height: 1.8;
    color: #333;
}
```

## OUTPUT

![alt text](<Screenshot (77).png>)

![alt text](<Screenshot (78).png>)

![alt text](<Screenshot (79).png>)

![alt text](<Screenshot (80).png>)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
