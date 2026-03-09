recruitment-website/
│
├─ index.html
├─ style.css
└─ script.js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dream Jobs Recruitment</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Dream Jobs Recruitment</h1>
        <nav>
            <ul>
                <li><a href="#jobs">Jobs</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="jobs">
        <h2>Available Positions</h2>
        <div class="job-list">
            <div class="job">
                <h3>Front-End Developer</h3>
                <p>Location: Central London | Full-time</p>
                <button onclick="applyJob('Front-End Developer')">Apply Now</button>
            </div>
            <div class="job">
                <h3>SEO Specialist</h3>
                <p>Location: Remote | Part-time</p>
                <button onclick="applyJob('SEO Specialist')">Apply Now</button>
            </div>
        </div>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>We connect top talent with the best companies. Update this section easily!</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contactForm">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2026 Dream Jobs Recruitment. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>

    <!-- Tawk.to Live Chat -->
    <script type="text/javascript">
        var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
        (function(){
            var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
            s1.async=true;
            s1.src='https://embed.tawk.to/69aebeeeddd7fc1c34853608/default';
            s1.charset='UTF-8';
            s1.setAttribute('crossorigin','*');
            s0.parentNode.insertBefore(s1,s0);
        })();
    </script>

</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    background-color: #f4f4f4;
}

header {
    background: #0073e6;
    color: white;
    padding: 20px 0;
    text-align: center;
}

header nav ul {
    list-style: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 40px;
    max-width: 900px;
    margin: auto;
    background: white;
    margin-bottom: 20px;
    border-radius: 10px;
}

.job {
    border: 1px solid #ddd;
    padding: 15px;
    margin: 10px 0;
    border-radius: 5px;
}

button {
    background: #0073e6;
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #005bb5;
}

footer {
    text-align: center;
    padding: 20px;
    background: #333;
    color: white;
}
// Apply Job Alert
function applyJob(jobTitle) {
    alert(`Thanks for applying to the ${jobTitle} position. We'll contact you soon!`);
}

// Contact Form Submission
document.getElementById('contactForm').addEventListener('submit', function(e){
    e.preventDefault();
    alert('Thank you! Your message has been sent.');
});
