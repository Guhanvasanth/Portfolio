# Ex01 Portfolio
## Name: Guhan Vasanth A 
## Reg No: 212225100014
## Date: 12.8.2026

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

## PROGRAM:

## index.html
```

```
## CSS
```
/* =========================================
   STYLE.CSS - TYLER DURDEN AESTHETIC
   ========================================= */

/* Import Fonts */
@import url('https://fonts.googleapis.com/css2?family=Anton&family=Inter:wght@300;400;600&display=swap');

/* Variables */
:root {
    --bg-color: #050505;       /* Deep Black */
    --text-color: #ffffff;     /* White */
    --acc<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gokul Sharan | Portfolio</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Anton&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        /* =========================================
           CSS RESET & BASE STYLES
           ========================================= */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --bg-color: #050505;
            --text-color: #ffffff;
            --accent-gray: #888888;
            --font-display: 'Anton', sans-serif;
            --font-body: 'Inter', sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: var(--font-body);
            overflow-x: hidden;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: all 0.3s ease;
        }

        /* =========================================
           UTILITY CLASSES
           ========================================= */
        .container {
            width: 88%;
            max-width: 1000px;
            margin: 0 auto;
            padding: 80px 0;
        }

        .section-title {
            font-family: var(--font-display);
            font-size: 4rem;
            text-transform: uppercase;
            margin-bottom: 40px;
            letter-spacing: 2px;
            border-bottom: 2px solid #222;
            padding-bottom: 10px;
        }

        /* =========================================
           HERO SECTION (HOME)
           ========================================= */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .hero-title {
            font-family: var(--font-display);
            font-size: clamp(3rem, 11vw, 8rem); /* Responsive Giant Text */
            text-transform: uppercase;
            line-height: 0.9;
            letter-spacing: -2px;
            margin-bottom: 20px;
            white-space: nowrap;
        }

        .hero-image-frame {
            width: 100%;
            max-width: 700px;
            aspect-ratio: 16/9;
            background-color: #111;
            margin-bottom: 30px;
            overflow: hidden;
            position: relative;
            /* The Gritty Filter Effect */
            filter: grayscale(100%) contrast(1.1) brightness(0.9);
            border: 1px solid #222;
        }

        .hero-image-frame img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        .hero-nav {
            display: flex;
            gap: 40px;
            margin-bottom: 30px;
        }

        .hero-nav a {
            font-size: 1.1rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            font-weight: 400;
        }

        .hero-nav a:hover {
            color: var(--accent-gray);
            text-decoration: line-through;
        }

        .tagline {
            font-size: 0.85rem;
            color: var(--accent-gray);
            text-transform: uppercase;
            letter-spacing: 4px;
        }

        /* =========================================
           ABOUT SECTION
           ========================================= */
        .about-text {
            font-size: 1.5rem;
            max-width: 800px;
            color: #ccc;
            line-height: 1.8;
            font-weight: 300;
        }

        .about-text strong {
            color: #fff;
            font-weight: 600;
        }

        /* =========================================
           WORK SECTION
           ========================================= */
        .work-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .project-card {
            background: #111;
            aspect-ratio: 1/1;
            position: relative;
            overflow: hidden;
            border: 1px solid #222;
            cursor: pointer;
        }

        .project-card:hover img {
            transform: scale(1.05);
            opacity: 0.5;
        }

        .project-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            filter: grayscale(100%);
            transition: transform 0.5s ease, opacity 0.5s ease;
        }

        .project-info {
            position: absolute;
            bottom: 20px;
            left: 20px;
            pointer-events: none;
        }

        .project-title {
            font-family: var(--font-display);
            font-size: 2rem;
            text-transform: uppercase;
            color: #fff;
        }

        .project-cat {
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: #aaa;
        }

        /* =========================================
           CONTACT SECTION
           ========================================= */
        .contact-area {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .email-link {
            font-family: var(--font-display);
            font-size: clamp(2rem, 5vw, 4rem);
            text-transform: uppercase;
            color: #fff;
            border-bottom: 1px solid transparent;
        }

        .email-link:hover {
            color: #aaa;
            border-bottom: 1px solid #aaa;
        }

        .socials {
            display: flex;
            gap: 20px;
            margin-top: 20px;
        }

        .socials a {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            border: 1px solid #333;
            padding: 10px 20px;
        }

        .socials a:hover {
            background: #fff;
            color: #000;
        }

        /* =========================================
           FOOTER
           ========================================= */
        footer {
            text-align: center;
            padding: 40px 0;
            border-top: 1px solid #111;
            margin-top: 80px;
            font-size: 0.75rem;
            color: #444;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* Mobile Adjustments */
        @media (max-width: 768px) {
            .hero-nav {
                flex-direction: column;
                gap: 15px;
            }
            .section-title {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>

    <section class="hero" id="home">
        <div class="container">
            <h1 class="hero-title">GOKUL SHARAN</h1>
            
            <div class="hero-image-frame">
                <img src="your-image.jpg" alt="Gokul Sharan Portrait">
            </div>

            <nav class="hero-nav">
                <a href="#about">About</a>
                <a href="#work">Work</a>
                <a href="#contact">Contact</a>
            </nav>

            <p class="tagline">Minimalist. Artist. Nihilist.</p>
        </div>
    </section>

    <section class="container" id="about">
        <h2 class="section-title">Who am I?</h2>
        <p class="about-text">
            I am a creator operating in the shadows of the digital realm. My work strips away the unnecessary, focusing only on raw structure and function. 
            <br><br>
            <strong>I do not design for comfort. I design for impact.</strong>
            <br><br>
            Like a copy of a copy, the web is full of noise. I am here to bring the silence. Based in Chennai, I specialize in web aesthetics that challenge the norm.
        </p>
    </section>

    <section class="container" id="work">
        <h2 class="section-title">Selected Works</h2>
        <div class="work-grid">
            <div class="project-card">
                <img src="https://images.unsplash.com/photo-1480796927426-f609979314bd?q=80&w=1000&auto=format&fit=crop" alt="Project 1">
                <div class="project-info">
                    <h3 class="project-title">Project Mayhem</h3>
                    <span class="project-cat">Web Design</span>
                </div>
            </div>

            <div class="project-card">
                <img src="https://images.unsplash.com/photo-1517487881594-2787fef5ebf7?q=80&w=1000&auto=format&fit=crop" alt="Project 2">
                <div class="project-info">
                    <h3 class="project-title">Paper Street</h3>
                    <span class="project-cat">Branding</span>
                </div>
            </div>

            <div class="project-card">
                <img src="https://images.unsplash.com/photo-1550684848-fac1c5b4e853?q=80&w=1000&auto=format&fit=crop" alt="Project 3">
                <div class="project-info">
                    <h3 class="project-title">Zero Hour</h3>
                    <span class="project-cat">Development</span>
                </div>
            </div>
             <div class="project-card">
                <img src="https://images.unsplash.com/photo-1494438639946-1ebd1d20bf85?q=80&w=1000&auto=format&fit=crop" alt="Project 4">
                <div class="project-info">
                    <h3 class="project-title">Soap Co.</h3>
                    <span class="project-cat">Product</span>
                </div>
            </div>
        </div>
    </section>

    <section class="container" id="contact">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-area">
            <p style="color: #888; margin-bottom: 10px;">READY TO BURN IT ALL DOWN?</p>
            <a href="mailto:gokztechz@gmail.com" class="email-link">GOKZTECHZ@GMAIL.COM</a>
            
            <div class="socials">
                <a href="#">Instagram</a>
                <a href="#">Twitter</a>
                <a href="#">LinkedIn</a>
            </div>
        </div>
    </section>

    <footer>
        &copy; 2025 Gokul Sharan. All Rights Reserved.
    </footer>

</body>
</html>ent-gray: #888888;    /* Muted Gray */
    --font-display: 'Anton', sans-serif;
    --font-body: 'Inter', sans-serif;
}

/* Base Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background-color: var(--bg-color);
    color: var(--text-color);
    font-family: var(--font-body);
    overflow-x: hidden;
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
    transition: all 0.3s ease;
}

/* =========================================
   UTILITY CLASSES
   ========================================= */
.container {
    width: 88%;
    max-width: 1000px;
    margin: 0 auto;
    padding: 80px 0;
}

.section-title {
    font-family: var(--font-display);
    font-size: 4rem;
    text-transform: uppercase;
    margin-bottom: 40px;
    letter-spacing: 2px;
    border-bottom: 2px solid #222;
    padding-bottom: 10px;
}

/* =========================================
   HERO SECTION (HOME)
   ========================================= */
.hero {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero-title {
    font-family: var(--font-display);
    font-size: clamp(3rem, 11vw, 8rem); /* Responsive Giant Text */
    text-transform: uppercase;
    line-height: 0.9;
    letter-spacing: -2px;
    margin-bottom: 20px;
    white-space: nowrap;
}

.hero-image-frame {
    width: 100%;
    max-width: 700px;
    aspect-ratio: 16/9;
    background-color: #111;
    margin-bottom: 30px;
    overflow: hidden;
    position: relative;
    /* The Gritty Filter Effect */
    filter: grayscale(100%) contrast(1.1) brightness(0.9);
    border: 1px solid #222;
}

.hero-image-frame img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

.hero-nav {
    display: flex;
    gap: 40px;
    margin-bottom: 30px;
}

.hero-nav a {
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-weight: 400;
}

.hero-nav a:hover {
    color: var(--accent-gray);
    text-decoration: line-through;
}

.tagline {
    font-size: 0.85rem;
    color: var(--accent-gray);
    text-transform: uppercase;
    letter-spacing: 4px;
}

/* =========================================
   ABOUT SECTION
   ========================================= */
.about-text {
    font-size: 1.5rem;
    max-width: 800px;
    color: #ccc;
    line-height: 1.8;
    font-weight: 300;
}

.about-text strong {
    color: #fff;
    font-weight: 600;
}

/* =========================================
   WORK SECTION
   ========================================= */
.work-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
}

.project-card {
    background: #111;
    aspect-ratio: 1/1;
    position: relative;
    overflow: hidden;
    border: 1px solid #222;
    cursor: pointer;
}

.project-card:hover img {
    transform: scale(1.05);
    opacity: 0.5;
}

.project-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: grayscale(100%);
    transition: transform 0.5s ease, opacity 0.5s ease;
}

.project-info {
    position: absolute;
    bottom: 20px;
    left: 20px;
    pointer-events: none;
}

.project-title {
    font-family: var(--font-display);
    font-size: 2rem;
    text-transform: uppercase;
    color: #fff;
    margin-bottom: 5px;
}

.project-cat {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: #aaa;
}

/* =========================================
   CONTACT SECTION
   ========================================= */
.contact-area {
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.email-link {
    font-family: var(--font-display);
    font-size: clamp(2rem, 5vw, 4rem);
    text-transform: uppercase;
    color: #fff;
    border-bottom: 1px solid transparent;
}

.email-link:hover {
    color: #aaa;
    border-bottom: 1px solid #aaa;
}

.socials {
    display: flex;
    gap: 20px;
    margin-top: 20px;
}

.socials a {
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    border: 1px solid #333;
    padding: 10px 20px;
    color: #fff;
}

.socials a:hover {
    background: #fff;
    color: #000;
}

/* =========================================
   FOOTER
   ========================================= */
footer {
    text-align: center;
    padding: 40px 0;
    border-top: 1px solid #111;
    margin-top: 80px;
    font-size: 0.75rem;
    color: #444;
    text-transform: uppercase;
    letter-spacing: 2px;
}

/* =========================================
   MEDIA QUERIES (RESPONSIVE)
   ========================================= */
@media (max-width: 768px) {
    .hero-nav {
        flex-direction: column;
        gap: 15px;
    }
    
    .section-title {
        font-size: 2.5rem;
    }
    
    .container {
        width: 90%;
        padding: 60px 0;
    }
}
```


## OUTPUT:

<img width="2013" height="1792" alt="Gemini_Generated_Image_vulhaqvulhaqvulh" src="https://github.com/user-attachments/assets/2067c020-1945-462e-a7cb-d2f0231ac23a" />










## RESULT:
The program for creating Portfolio using HTML and CSS is executed successfully.
