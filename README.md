# Ex01 Portfolio
## Name : Guhan Vasanth A 
## reg no : 212225100014

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



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guhan Vasanth A- Portfolio</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; background-color: #f5f5f5; color: #333; }
        header { background: #4CAF50; color: white; padding: 20px; text-align: center; }
        section { padding: 20px; max-width: 900px; margin: auto; }
        .skills span { display: inline-block; background: #e0e0e0; padding: 5px 10px; margin: 5px; border-radius: 5px; }
        .card { background: white; padding: 15px; border-radius: 5px; margin-bottom: 15px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        footer { background: #333; color: white; text-align: center; padding: 10px; margin-top: 20px; }
    </style>
</head>
<body>
    <header>
        <h1>Guhan Vasanth A</h1>
        <p>B.Tech IT - 2nd Year | Saveetha Engineering College</p>
    </header>

    <section>
        <div class="card">
            <h2>About Me</h2>
            <p>Hi, I'm Guhan Vasanth A , currently pursuing my B.Tech cse(cs) at Saveetha Engineering College. I'm passionate about web development, UI/UX design, and constantly learning new technologies. I have completed a 2-month internship at a software company, gaining practical experience in the tech industry.</p>
        </div>

        <div class="card">
            <h2>Skills</h2>
            <div class="skills">
                <span>Web Development</span>
                <span>UI/UX Design</span>
                <span>Python (Basics)</span>
                <span>C (Basics)</span>
                <span>JavaScript (Basics)</span>
                <span>HTML & CSS</span>
            </div>
        </div>
    </section>

    <footer>
        <p>© 2026 Guhan Vasanth A </p>
    </footer>
</body>
</html>
