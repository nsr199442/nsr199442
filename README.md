
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080b14">
<meta name="description" content="Nishad Saranga Ranathunga — Workflow Automation, AI Assistant Development and Project Coordination.">
<title>Nishad Saranga Ranathunga | Portfolio</title>

<style>
:root {
    --bg: #080b14;
    --surface: rgba(255,255,255,0.045);
    --border: rgba(255,255,255,0.10);
    --text: #f2f4fa;
    --muted: #9ba5b8;
    --accent: #8b7cff;
    --cyan: #50d9e8;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 90px;
}

body {
    background: var(--bg);
    color: var(--text);
    font-family: Inter, "Segoe UI", Arial, sans-serif;
    line-height: 1.7;
    overflow-x: hidden;
}

/* Animated background */

.background {
    position: fixed;
    inset: 0;
    z-index: -2;
    overflow: hidden;
    pointer-events: none;
}

.orb {
    position: absolute;
    width: 450px;
    height: 450px;
    border-radius: 50%;
    filter: blur(110px);
    opacity: .17;
    animation: float 12s ease-in-out infinite alternate;
}

.orb.one {
    background: #7659ff;
    top: -180px;
    left: -100px;
}

.orb.two {
    background: #00bcd4;
    right: -180px;
    top: 40%;
    animation-delay: -5s;
}

.orb.three {
    background: #6439a8;
    bottom: -250px;
    left: 30%;
    animation-delay: -8s;
}

@keyframes float {
    from { transform: translate(0,0) scale(1); }
    to { transform: translate(80px,60px) scale(1.2); }
}

/* Navigation */

nav {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 100;
    background: rgba(8,11,20,.78);
    backdrop-filter: blur(18px);
    border-bottom: 1px solid var(--border);
}

.nav-inner {
    max-width: 1150px;
    margin: auto;
    padding: 18px 25px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-weight: 800;
    font-size: 19px;
    letter-spacing: -1px;
}

.logo span {
    color: var(--accent);
}

.nav-links {
    display: flex;
    gap: 28px;
    list-style: none;
}

.nav-links a {
    text-decoration: none;
    color: var(--muted);
    font-size: 13px;
    transition: .3s;
}

.nav-links a:hover {
    color: white;
}

/* Main layout */

.container {
    max-width: 1050px;
    margin: auto;
    padding: 0 25px;
}

section {
    padding: 105px 0 30px;
}

.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    padding-top: 120px;
}

.hero-content {
    max-width: 850px;
}

.availability {
    display: inline-flex;
    align-items: center;
    gap: 9px;
    border: 1px solid var(--border);
    padding: 7px 15px;
    border-radius: 50px;
    color: var(--muted);
    font-size: 12px;
    margin-bottom: 30px;
    animation: fadeUp 1s both;
}

.dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    background: #48db9a;
    box-shadow: 0 0 12px #48db9a;
}

h1 {
    font-size: clamp(42px, 7vw, 78px);
    line-height: 1.08;
    letter-spacing: -4px;
    font-weight: 800;
    animation: fadeUp 1s .15s both;
}

.gradient {
    background: linear-gradient(100deg, #a69aff, #57dce9);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.hero-subtitle {
    font-size: clamp(16px, 2vw, 20px);
    color: var(--muted);
    margin-top: 25px;
    animation: fadeUp 1s .3s both;
}

.hero-description {
    color: #a5afc0;
    max-width: 680px;
    margin-top: 22px;
    font-size: 15px;
    animation: fadeUp 1s .45s both;
}

.hero-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    margin-top: 35px;
    animation: fadeUp 1s .6s both;
}

.btn {
    display: inline-block;
    padding: 12px 23px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 13px;
    transition: .3s;
}

.btn-primary {
    background: linear-gradient(100deg, #8270ff, #4dbbdb);
    color: #080b14;
}

.btn-secondary {
    border: 1px solid var(--border);
    color: white;
}

.btn:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 30px rgba(125,100,255,.2);
}

.scroll-hint {
    margin-top: 75px;
    font-size: 11px;
    letter-spacing: 3px;
    color: #647086;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    50% { opacity: .35; }
}

/* Section headings */

.section-label {
    color: var(--cyan);
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 4px;
    text-transform: uppercase;
    margin-bottom: 12px;
}

.section-title {
    font-size: clamp(29px, 4vw, 43px);
    letter-spacing: -1.5px;
    margin-bottom: 25px;
}

.section-description {
    color: var(--muted);
    max-width: 750px;
    font-size: 15px;
}

/* Cards */

.grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    margin-top: 35px;
}

.card {
    position: relative;
    padding: 28px;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 15px;
    transition: .35s ease;
    overflow: hidden;
}

.card::before {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(139,124,255,.09), transparent 60%);
    opacity: 0;
    transition: .4s;
}

.card:hover {
    transform: translateY(-7px);
    border-color: rgba(139,124,255,.5);
    box-shadow: 0 15px 45px rgba(0,0,0,.2);
}

.card:hover::before {
    opacity: 1;
}

.card h3 {
    position: relative;
    font-size: 19px;
    margin-bottom: 13px;
}

.card p {
    position: relative;
    color: var(--muted);
    font-size: 13px;
}

.card-number {
    color: var(--accent);
    font-size: 12px;
    font-weight: 800;
    letter-spacing: 2px;
    margin-bottom: 15px;
}

/* Expertise */

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 30px;
}

.skill {
    padding: 10px 16px;
    border-radius: 7px;
    background: var(--surface);
    border: 1px solid var(--border);
    font-size: 13px;
    color: #c4cbe0;
    transition: .3s;
}

.skill:hover {
    border-color: var(--accent);
    color: white;
    transform: translateY(-3px);
}

/* Leadership */

.leadership {
    border-left: 2px solid var(--accent);
    padding: 10px 0 10px 30px;
    margin-top: 30px;
}

.leadership h3 {
    font-size: 23px;
    margin-bottom: 12px;
}

.leadership ul {
    margin: 20px 0 0 20px;
    color: var(--muted);
    font-size: 14px;
}

.leadership li {
    padding: 5px 0;
}

/* Notice */

.notice {
    margin-top: 25px;
    padding: 16px 20px;
    background: rgba(139,124,255,.07);
    border: 1px solid rgba(139,124,255,.2);
    border-radius: 9px;
    color: #aeb7cc;
    font-size: 12px;
}

/* Contact */

.contact-card {
    padding: 45px;
    text-align: center;
    border-radius: 18px;
    border: 1px solid var(--border);
    background: linear-gradient(135deg, rgba(139,124,255,.10), rgba(80,217,232,.04));
    margin-top: 30px;
}

.contact-card h2 {
    font-size: 32px;
    margin-bottom: 12px;
}

.contact-card p {
    color: var(--muted);
    font-size: 14px;
}

footer {
    text-align: center;
    padding: 55px 20px 30px;
    color: #667086;
    font-size: 12px;
}

/* Scroll reveal */

.reveal {
    opacity: 0;
    transform: translateY(35px);
    transition: opacity .8s ease, transform .8s ease;
}

.reveal.visible {
    opacity: 1;
    transform: translateY(0);
}

@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(25px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Mobile */

@media(max-width: 700px) {
    .nav-links {
        gap: 12px;
    }

    .nav-links a {
        font-size: 11px;
    }

    .grid {
        grid-template-columns: 1fr;
    }

    h1 {
        letter-spacing: -2px;
    }

    section {
        padding-top: 80px;
    }

    .contact-card {
        padding: 30px 18px;
    }
}

@media(max-width: 420px) {
    .nav-inner {
        padding: 14px 15px;
    }

    .logo {
        font-size: 15px;
    }

    .nav-links {
        gap: 9px;
    }

    .nav-links a {
        font-size: 10px;
    }
}

/* Accessibility */

@media(prefers-reduced-motion: reduce) {
    *, *::before, *::after {
        animation-duration: .01ms !important;
        animation-iteration-count: 1 !important;
        scroll-behavior: auto !important;
        transition-duration: .01ms !important;
    }

    .reveal {
        opacity: 1;
        transform: none;
    }
}
</style>
</head>

<body>

<div class="background">
    <div class="orb one"></div>
    <div class="orb two"></div>
    <div class="orb three"></div>
</div>

<nav>
    <div class="nav-inner">
        <div class="logo">NISHAD<span>.</span></div>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#expertise">Expertise</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </div>
</nav>

<main class="container">

<!-- HERO -->

<section class="hero">
    <div class="hero-content">

        <div class="availability">
            <span class="dot"></span>
            OPEN TO REMOTE & INTERNATIONAL OPPORTUNITIES
        </div>

        <h1>
            Hi, I'm<br>
            <span class="gradient">Nishad Saranga</span><br>
            Ranathunga.
        </h1>

        <div class="hero-subtitle">
            Workflow Automation · AI Assistant Development · Project Coordination
        </div>

        <p class="hero-description">
            I transform complex business processes into intelligent,
            connected systems. Exploring the intersection of automation,
            artificial intelligence, creative problem-solving and software development.
        </p>

        <div class="hero-buttons">
            <a href="#projects" class="btn btn-primary">Explore My Work ↗</a>
            <a href="https://www.linkedin.com/in/nishad-saranga/"
               target="_blank" rel="noopener noreferrer"
               class="btn btn-secondary">Connect With Me ↗</a>
        </div>

        <div class="scroll-hint">SCROLL TO EXPLORE ↓</div>

    </div>
</section>

<!-- ABOUT -->

<section id="about" class="reveal">
    <div class="section-label">01 / INTRODUCTION</div>
    <h2 class="section-title">A little about me.</h2>

    <p class="section-description">
        I have approximately 1.5 years of experience designing intelligent
        automation systems and AI-powered communication assistants.

        <br><br>

        My work focuses on understanding business processes, transforming
        manual operations into automated workflows, connecting different
        systems, and developing intelligent solutions that simplify everyday tasks.

        <br><br>

        I also explore advanced AI-assisted development approaches to turn
        ideas into functional prototypes, experiment with unconventional
        solutions, and accelerate software development.
    </p>
</section>

<!-- EXPERTISE -->

<section id="expertise" class="reveal">
    <div class="section-label">02 / CAPABILITIES</div>
    <h2 class="section-title">What I work with.</h2>

    <p class="section-description">
        A combination of technical thinking, automation design,
        intelligent systems and project coordination.
    </p>

    <div class="skills">
        <span class="skill">Intelligent Workflow Design</span>
        <span class="skill">AI-Powered Assistants</span>
        <span class="skill">Business Process Optimization</span>
        <span class="skill">System Integration</span>
        <span class="skill">Automated Communication</span>
        <span class="skill">AI-Assisted Prototyping</span>
        <span class="skill">Requirements Analysis</span>
        <span class="skill">Project Coordination</span>
        <span class="skill">Technical Documentation</span>
        <span class="skill">Data Flow Management</span>
    </div>
</section>

<!-- PROJECTS -->

<section id="projects" class="reveal">
    <div class="section-label">03 / SELECTED WORK</div>
    <h2 class="section-title">Ideas into systems.</h2>

    <p class="section-description">
        A selection of workflow experiments and intelligent system concepts
        developed to explore practical solutions to real-world problems.
    </p>

    <div class="grid">

        <div class="card">
            <div class="card-number">PROJECT 01</div>
            <h3>Intelligent Learning Assistant</h3>
            <p>
                Designed a conversational learning assistant capable of
                identifying student progress, monitoring learning activities,
                and responding through both text and voice.

                <br><br>
                An interactive approach to educational progress tracking.
            </p>
        </div>

        <div class="card">
            <div class="card-number">PROJECT 02</div>
            <h3>Automated Ordering Assistant</h3>
            <p>
                Developed an AI-powered ordering workflow handling product
                inquiries, catalog navigation, shopping cart operations,
                and order collection through conversational interactions.

                <br><br>
                Reimagining traditional ordering experiences.
            </p>
        </div>

        <div class="card">
            <div class="card-number">PROJECT 03</div>
            <h3>Automated Financial Notifications</h3>
            <p>
                Designed an automated system for generating financial
                receipts and delivering notifications through scheduled
                communication processes.

                <br><br>
                Connecting document generation with instant communication.
            </p>
        </div>

    </div>

    <div class="notice">
        Note: These projects represent configured prototypes and development
        experiments. They were not fully deployed into production, and no
        measured business outcomes are claimed.
    </div>
</section>

<!-- LEADERSHIP -->

<section id="leadership" class="reveal">
    <div class="section-label">04 / PROJECT LEADERSHIP</div>
    <h2 class="section-title">Beyond development.</h2>

    <div class="leadership">
        <h3>Bexvis — Project Manager</h3>

        <p class="section-description">
            Led the planning and coordination of a technology-driven project
            involving intelligent visual analysis and real-time data processing.
        </p>

        <ul>
            <li>Designed the overall project blueprint.</li>
            <li>Defined core calculation logic and operational rules.</li>
            <li>Coordinated technical activities across the project team.</li>
            <li>Structured requirements and implementation objectives.</li>
            <li>Guided project direction from concept toward technical development.</li>
        </ul>

        <div class="notice">
            My contribution focused on project architecture, planning,
            calculation logic and coordination. Specialized technical
            components were implemented by the development team.
        </div>
    </div>
</section>

<!-- CAREER -->

<section class="reveal">
    <div class="section-label">05 / THE NEXT CHAPTER</div>
    <h2 class="section-title">Where I'm heading.</h2>

    <p class="section-description">
        I'm interested in opportunities where I can combine automation
        thinking, AI-assisted development, problem-solving and project
        coordination to build meaningful solutions.

        <br><br>

        Currently open to:
    </p>

    <div class="skills">
        <span class="skill">Remote Opportunities</span>
        <span class="skill">AI Assistant Development</span>
        <span class="skill">Workflow Automation</span>
        <span class="skill">Automation Consulting</span>
        <span class="skill">Project Coordination</span>
        <span class="skill">International Relocation</span>
        <span class="skill">Employer Visa Sponsorship</span>
    </div>
</section>

<!-- CONTACT -->

<section id="contact" class="reveal">
    <div class="contact-card">
        <div class="section-label">06 / GET IN TOUCH</div>

        <h2>Have an idea?</h2>

        <p>
            Let's explore what we can build together.
            I'm always interested in meaningful projects,
            new challenges and opportunities.
        </p>

        <div class="hero-buttons" style="justify-content:center">
            <a href="https://www.linkedin.com/in/nishad-saranga/"
               target="_blank" rel="noopener noreferrer"
               class="btn btn-primary">
                Connect on LinkedIn ↗
            </a>
        </div>
    </div>
</section>

</main>

<footer>
    <p>© <span id="year"></span> Nishad Saranga Ranathunga.</p>
    <p>Designed with curiosity. Built with intention.</p>
</footer>

<script>
// Automatic copyright year
document.getElementById("year").textContent =
    new Date().getFullYear();

// Scroll reveal animation
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add("visible");
            observer.unobserve(entry.target);
        }
    });
}, {
    threshold: 0.12
});

document.querySelectorAll(".reveal").forEach(element => {
    observer.observe(element);
});
</script>

</body>
</html>
