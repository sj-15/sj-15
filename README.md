<!DOCTYPE html>
<html>
<head>
    <title>Sourav's Portfolio</title>
    <style>
        /* Global styles */
        body {
            margin: 0;
            padding: 0;
            font-family: sans-serif;
        }

        h1 {
            font-size: 3rem;
            margin-top: 1.5rem;
        }

        h2 {
            font-size: 2rem;
            margin-top: 2.5rem;
        }

        h3 {
            font-size: 1.5rem;
            margin-top: 2rem;
        }

        ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        li {
            display: inline-block;
            margin-right: 1rem;
        }

        a {
            text-decoration: none;
            color: #000;
            transition: all 0.3s ease-in-out;
        }

        a:hover {
            color: #0077b5;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 2rem;
            text-align: center;
        }

        #typing {
            display: inline-block;
        }

        #cursor {
            display: inline-block;
            animation: blink 0.7s infinite;
        }

        @keyframes blink {
            50% {
                opacity: 0;
            }
        }

        .tech-stack {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: 2rem;
        }

        .tech-stack img {
            margin: 0 1rem;
            filter: grayscale(100%);
            transition: all 0.3s ease-in-out;
        }

        .tech-stack img:hover {
            filter: grayscale(0);
        }

        .project {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 2rem;
        }

        .project-item {
            width: 250px;
            margin: 1rem;
            padding: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease-in-out;
        }

        .project-item:hover {
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
        }

        .learning {
            margin-top: 2rem;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Hey there!👋 I'm Sourav</h2>
        <hr>
        <ul>
            <li>
                <a href="https://www.linkedin.com/in/sourav-jana15/"><img
                        src="https://cdn.worldvectorlogo.com/logos/linkedin-icon-2.svg" alt="LinkedIn" width="30"
                        height="30"></a>
            </li>
            <li>
                <a href="sj15sourav@gmail.com"><img src="https://cdn.worldvectorlogo.com/logos/gmail-icon.svg"
                        alt="Gmail" width="30" height="30"></a>
            </li>
        </ul>
        <h3><span id="typing"></span><span id="cursor"></span></h3>
        <div>
            <h3>About Me</h3>
            <hr>
            <p>Currently in 3rd year pursuing B. Tech in Computer Science & Engineering from Dr. B. C. Roy Engineering
                College, Durgapur. I'm the vice president of iCoders' the official tech club of our college. I'm
                passionate about Competitive Coding, and enjoy solving puzzles like sudoku, rubix cube, etc. in the free
                time.</p>
        </div>
        <h3>Tech Stack</h3>
        <hr>
        <div class="tech-stack">
            <img src="https://cdn.iconscout.com/icon/free/png-256/c-programming-569564.png" alt="C++" height="50"
                width="50">
            <img src="https://cdn.iconscout.com/icon/free/png-256/python-2-226051.png" alt="Python" height="50"
                width="50">
            <img src="https://cdn.iconscout.com/icon/free/png-256/flutter-2038877-1720090.png" alt="Flutter" height="50"
                width="50">
            <img src="https://cdn.iconscout.com/icon/free/png-256/node-js-1-1174935.png" alt="Node.js" height="50"
                width="50">
            <img src="https://cdn.iconscout.com/icon/free/png-256/firebase-1-282796.png" alt="Firebase" height="50"
                width="50">
            <img src="https://cdn.iconscout.com/icon/free/png-256/mysql-19-1174939.png" alt="MySql" height="50"
                width="50">
        </div>
        <h3>Projects</h3>
        <hr>
        <div class="project">
            <div class="project-item">
                <h3>!non</h3>
                <p>A chatting platform: that two unknown users talk to each other with same interests without sharing
                    any kind of personal information like name, address, email, phone no, etc.</p>
            </div>
            <div class="project-item">
                <h3>tashveer</h3>
                <p>Create a photo-sharing app:
                    integrating with cloud
                    storage services like Google
                    Drive or Dropbox,
                    implementing social sharing
                    features, and using image
                    processing libraries like
                    Glide or Picasso.</p>
            </div>
            <div class="project-item">
                <h3>Project 3</h3>
                <p>Nunc aliquet orci enim, non rhoncus velit semper eu. Sed et mauris orci.</p>
            </div>
            <div class="project-item">
                <h3>Project 4</h3>
                <p>Fusce mattis gravida enim, vitae commodo elit dignissim vitae.</p>
            </div>
        </div>
        <div class="learning">
            <h3>What I'm Learning</h3>
            <hr>
            <p>Everday I try to learn something new. Currently I'm learning JavaScript from scratch. Also studying about
                DBMS and implementing using MySql.
            </p>
        </div>
        <h3>Thanks for stopping by!</h3>
    </div>
    <script>
        // Typing animation
        const words = ["A Fullstack Developer", "A Competitive Programmer"];
        let i = 0;
        let j = 0;
        let currentWord = "";
        let currentLetter = "";
        (function type() {
            if (i === words.length) {
                i = 0;
            }
            currentWord = words[i];
            currentLetter = currentWord.slice(0, ++j);
            document.getElementById("typing").textContent = currentLetter;
            if (currentLetter.length === currentWord.length) {
                i++;
                j = 0;
            }
            setTimeout(type, 100);

        })();
    </script>

</body>
</html>
