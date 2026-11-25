<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mst. Sadia Zaman Oishi | CSE Portfolio</title>

<meta name="description" content="Portfolio of Mst. Sadia Zaman Oishi, CSE student at IUBAT.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

/* ===== GLOBAL ===== */

:root {
    --bg: #0b071b;
    --card: #17102e;
    --purple: #8957ff;
    --pink: #ff55a5;
    --cyan: #36d9d0;
    --white: #ffffff;
    --muted: #aaa1c4;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 85px;
}

body {
    font-family: 'Outfit', sans-serif;
    background: var(--bg);
    color: var(--white);
    line-height: 1.7;
    overflow-x: hidden;
}

a {
    text-decoration: none;
    color: inherit;
}

.container {
    width: 88%;
    max-width: 1150px;
    margin: auto;
}

section {
    padding: 100px 0;
}

.section-title {
    text-align: center;
    font-size: 38px;
    font-weight: 800;
    margin-bottom: 10px;
}

.section-title span {
    color: var(--purple);
}

.section-subtitle {
    text-align: center;
    color: var(--muted);
    margin-bottom: 55px;
}

/* ===== NAVBAR ===== */

nav {
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(11, 7, 27, 0.88);
    backdrop-filter: blur(18px);
    border-bottom: 1px solid rgba(255,255,255,0.08);
}

.nav-inner {
    width: 88%;
    max-width: 1150px;
    margin: auto;
    min-height: 75px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
}

.logo {
    font-size: 27px;
    font-weight: 800;
    background: linear-gradient(90deg, var(--purple), var(--pink));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.nav-links {
    display: flex;
    gap: 28px;
}

.nav-links a {
    color: #d6cfea;
    font-weight: 500;
    transition: .3s;
}

.nav-links a:hover {
    color: var(--pink);
}

/* ===== HERO ===== */

.hero {
    min-height: 680px;
    display: flex;
    align-items: center;
    position: relative;
    overflow: hidden;
    background:
        radial-gradient(circle at 85% 35%, rgba(137,87,255,.19), transparent 35%),
        radial-gradient(circle at 10% 85%, rgba(255,85,165,.12), transparent 30%);
}

.hero-inner {
    display: grid;
    grid-template-columns: 1.3fr 1fr;
    align-items: center;
    gap: 50px;
}

.role {
    display: inline-block;
    color: var(--cyan);
    background: rgba(54,217,208,.09);
    border: 1px solid rgba(54,217,208,.3);
    padding: 8px 18px;
    border-radius: 30px;
    margin-bottom: 22px;
    font-size: 14px;
}

.hero h1 {
    font-size: clamp(42px, 6vw, 68px);
    line-height: 1.12;
    font-weight: 800;
    margin-bottom: 22px;
}

.hero h1 span {
    background: linear-gradient(90deg, var(--purple), var(--pink));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.hero p {
    color: var(--muted);
    font-size: 17px;
    max-width: 520px;
    margin-bottom: 32px;
}

.buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
}

.btn {
    padding: 13px 27px;
    border-radius: 35px;
    font-weight: 600;
    display: inline-block;
    transition: .3s;
}

.btn-primary {
    background: linear-gradient(90deg, var(--purple), var(--pink));
    color: white;
    box-shadow: 0 8px 25px rgba(137,87,255,.25);
}

.btn-outline {
    border: 1px solid rgba(255,255,255,.3);
    color: white;
}

.btn:hover {
    transform: translateY(-4px);
}

/* PROFILE IMAGE */

.photo-area {
    display: flex;
    justify-content: center;
}

.photo {
    width: min(340px, 75vw);
    aspect-ratio: 1;
    border-radius: 50%;
    padding: 10px;
    background: linear-gradient(135deg, var(--purple), var(--pink), var(--cyan));
    box-shadow: 0 0 60px rgba(137,87,255,.25);
    animation: float 4s ease-in-out infinite;
}

.photo img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
    border: 6px solid var(--bg);
}

.photo-fallback {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    background: var(--card);
    border: 6px solid var(--bg);
    display: grid;
    place-items: center;
    font-size: 85px;
    font-weight: 800;
    color: var(--pink);
}

@keyframes float {
    0%,100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
}

/* ===== ABOUT ===== */

.about-content {
    max-width: 850px;
    margin: auto;
    padding: 40px;
    border-radius: 25px;
    background: linear-gradient(145deg, #1b1236, #110b25);
    border: 1px solid rgba(255,255,255,.08);
    box-shadow: 0 15px 45px rgba(0,0,0,.2);
}

.about-content p {
    color: var(--muted);
    margin-bottom: 18px;
    font-size: 17px;
}

.facts {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 25px;
}

.facts span {
    padding: 9px 18px;
    border-radius: 30px;
    background: rgba(137,87,255,.14);
    border: 1px solid rgba(137,87,255,.3);
    color: #d9c9ff;
    font-size: 14px;
}

/* ===== EDUCATION ===== */

.edu-card {
    max-width: 750px;
    margin: auto;
    padding: 35px;
    background: var(--card);
    border-radius: 20px;
    border-left: 5px solid var(--purple);
    transition: .3s;
}

.edu-card:hover {
    transform: translateY(-5px);
}

.edu-card h3 {
    font-size: 23px;
    margin-bottom: 10px;
}

.edu-card .where {
    color: var(--pink);
    font-weight: 600;
    margin-bottom: 12px;
}

.edu-card p {
    color: var(--muted);
}

/* ===== SKILLS ===== */

.skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
}

.skill-card {
    background: var(--card);
    padding: 32px 25px;
    border-radius: 20px;
    border: 1px solid rgba(255,255,255,.07);
    transition: .3s;
}

.skill-card:hover {
    transform: translateY(-8px);
    border-color: var(--purple);
    box-shadow: 0 10px 35px rgba(137,87,255,.12);
}

.skill-icon {
    font-size: 35px;
    margin-bottom: 15px;
}

.skill-card h3 {
    margin-bottom: 15px;
    font-size: 21px;
}

.tags {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
}

.tags span {
    background: rgba(137,87,255,.15);
    color: #d8caff;
    padding: 6px 14px;
    border-radius: 20px;
    font-size: 13px;
}

/* ===== PROJECTS ===== */

.projects-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 25px;
}

.project-card {
    background: var(--card);
    padding: 32px;
    border-radius: 22px;
    border: 1px solid rgba(255,255,255,.08);
    transition: .3s;
}

.project-card:hover {
    transform: translateY(-8px);
    border-color: var(--pink);
    box-shadow: 0 12px 35px rgba(255,85,165,.1);
}

.project-number {
    font-size: 35px;
    font-weight: 800;
    color: var(--purple);
    margin-bottom: 15px;
}

.project-card h3 {
    font-size: 22px;
    margin-bottom: 12px;
}

.project-card p {
    color: var(--muted);
    margin-bottom: 22px;
}

.project-link {
    color: var(--pink);
    font-weight: 600;
}

/* ===== CONTACT ===== */

.contact-box {
    background: linear-gradient(135deg, #27134f, #17102e);
    border: 1px solid rgba(137,87,255,.3);
    padding: 55px 30px;
    border-radius: 28px;
    text-align: center;
}

.contact-box p {
    color: var(--muted);
    margin: 12px 0 30px;
}

.links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 14px;
}

.links a {
    padding: 12px 23px;
    border-radius: 30px;
    background: var(--purple);
    color: white;
    font-weight: 600;
    transition: .3s;
}

.links a:hover {
    background: var(--pink);
    transform: translateY(-4px);
}

/* ===== FOOTER ===== */

footer {
    text-align: center;
    padding: 30px 15px;
    color: var(--muted);
    border-top: 1px solid rgba(255,255,255,.08);
    font-size: 14px;
}

/* ===== RESPONSIVE ===== */

@media(max-width: 850px) {

    .hero-inner {
        grid-template-columns: 1fr;
        text-align: center;
    }

    .hero p {
        margin-left: auto;
        margin-right: auto;
    }

    .buttons {
        justify-content: center;
    }

    .photo-area {
        grid-row: 1;
    }

    .photo {
        width: min(260px, 65vw);
    }

    .skills-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .nav-links {
        gap: 15px;
    }
}

@media(max-width: 600px) {

    section {
        padding: 75px 0;
    }

    .nav-inner {
        flex-direction: column;
        padding: 13px 0;
        gap: 8px;
    }

    .nav-links {
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
        gap: 10px 17px;
        font-size: 13px;
    }

    .hero {
        min-height: auto;
        padding: 60px 0 80px;
    }

    .hero h1 {
        font-size: 42px;
    }

    .section-title {
        font-size: 31px;
    }

    .skills-grid,
    .projects-grid {
        grid-template-columns: 1fr;
    }

    .about-content {
        padding: 25px;
    }

    .edu-card {
        padding: 25px;
    }

    .contact-box {
        padding: 40px 20px;
    }
}

@media(prefers-reduced-motion: reduce) {
    *, *::before, *::after {
        animation: none !important;
        scroll-behavior: auto !important;
        transition: none !important;
    }
}

</style>
</head>

<body>

<!-- NAVBAR -->

<nav>
    <div class="nav-inner">

        <a href="#home" class="logo">Oishi.</a>

        <div class="nav-links">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </div>

    </div>
</nav>


<!-- HERO SECTION -->

<header class="hero" id="home">

    <div class="container hero-inner">

        <div class="hero-text">

            <div class="role">
                CSE Student at IUBAT
            </div>

            <h1>
                Hi, I'm <br>
                <span>Mst. Sadia Zaman Oishi</span>
            </h1>

            <p>
                I build small projects with code and keep learning every day.
                Currently focused on programming fundamentals and web development.
            </p>

            <div class="buttons">

                <a href="#contact" class="btn btn-primary">
                    Contact Me
                </a>

                <a href="#projects" class="btn btn-outline">
                    View Projects
                </a>

            </div>

        </div>


        <div class="photo-area">

            <div class="photo">

                <img
                    src="profile.jpg"
                    alt="Photo of Mst. Sadia Zaman Oishi"
                    onerror="this.outerHTML='<div class=&quot;photo-fallback&quot;>O</div>'"
                >

            </div>

        </div>

    </div>

</header>


<!-- ABOUT -->

<section id="about">

    <div class="container">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <p class="section-subtitle">
            Get to know me better
        </p>

        <div class="about-content">

            <p>
                I'm a Computer Science and Engineering student at
                International University of Business Agriculture and Technology (IUBAT).
                I enjoy solving problems, learning how software works,
                and sharing what I build.
            </p>

            <p>
                I'm learning the C programming language and exploring
                mobile app development, game development, AI and cybersecurity
                to find the field I want to specialize in.
            </p>

            <div class="facts">

                <span>CSE Student</span>
                <span>IUBAT</span>
                <span>C Programming</span>
                <span>Web Basics</span>

            </div>

        </div>

    </div>

</section>


<!-- EDUCATION -->

<section id="education">

    <div class="container">

        <h2 class="section-title">
            My <span>Education</span>
        </h2>

        <p class="section-subtitle">
            My academic journey
        </p>

        <div class="edu-card">

            <h3>
                Computer Science and Engineering (CSE)
            </h3>

            <div class="where">
                International University of Business Agriculture and Technology (IUBAT)
            </div>

            <p>
                Studying programming, problem solving and the fundamentals
                of computer science.
            </p>

        </div>

    </div>

</section>


<!-- SKILLS -->

<section id="skills">

    <div class="container">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>

        <p class="section-subtitle">
            Technologies and tools I'm learning
        </p>

        <div class="skills-grid">

            <div class="skill-card">

                <div class="skill-icon">💻</div>

                <h3>Programming</h3>

                <div class="tags">
                    <span>C</span>
                </div>

            </div>


            <div class="skill-card">

                <div class="skill-icon">🌐</div>

                <h3>Web Development</h3>

                <div class="tags">
                    <span>HTML</span>
                    <span>CSS</span>
                </div>

            </div>


            <div class="skill-card">

                <div class="skill-icon">⚙️</div>

                <h3>Tools</h3>

                <div class="tags">
                    <span>Git</span>
                    <span>GitHub</span>
                    <span>GitHub Pages</span>
                </div>

            </div>

        </div>

    </div>

</section>


<!-- PROJECTS -->

<section id="projects">

    <div class="container">

        <h2 class="section-title">
            My <span>Projects</span>
        </h2>

        <p class="section-subtitle">
            Things I've built so far
        </p>

        <div class="projects-grid">

            <div class="project-card">

                <div class="project-number">01</div>

                <h3>Personal Portfolio Website</h3>

                <p>
                    This responsive website, built with HTML and CSS
                    and hosted for free on GitHub Pages.
                </p>

                <a
                    class="project-link"
                    href="https://github.com/sadiaoishi/sadiaoishi.github.io"
                    target="_blank"
                    rel="noopener"
                >
                    View Source on GitHub →
                </a>

            </div>


            <div class="project-card">

                <div class="project-number">02</div>

                <h3>C Practice Programs</h3>

                <p>
                    Small C programs such as arithmetic operations
                    and percentage calculation while learning the language.
                </p>

                <span class="project-link">
                    Learning Project
                </span>

            </div>

        </div>

    </div>

</section>


<!-- CONTACT -->

<section id="contact">

    <div class="container">

        <div class="contact-box">

            <h2 class="section-title">
                Get In <span>Touch</span>
            </h2>

            <p>
                Feel free to reach out. I'd love to hear from you.
            </p>

            <div class="links" id="links"></div>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    © 2026 Mst. Sadia Zaman Oishi.
    Built with HTML and CSS by Shahariar Ahmed Nayem.

</footer>


<!-- CONTACT DETAILS -->

<script>

const CONTACT = {

    email: "",
    phone: "",
    linkedin: "",
    facebook: "",
    cv: ""

};

const items = [

    [CONTACT.email, "Email", "mailto:" + CONTACT.email],

    [CONTACT.phone, "Call", "tel:" + CONTACT.phone],

    [CONTACT.linkedin, "LinkedIn", CONTACT.linkedin],

    [CONTACT.facebook, "Facebook", CONTACT.facebook],

    [CONTACT.cv, "Download CV", CONTACT.cv],

    ["x", "GitHub", "https://github.com/sadiaoishi"]

];

const box = document.getElementById("links");

items.forEach(([value, label, href]) => {

    if (!value) return;

    const link = document.createElement("a");

    link.textContent = label;
    link.href = href;

    if (href.startsWith("http")) {
        link.target = "_blank";
        link.rel = "noopener";
    }

    box.appendChild(link);

});

</script>

</body>
</html>



