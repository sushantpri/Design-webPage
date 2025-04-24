# Design-webPage
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>HashedBit Assignment</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: sans-serif;
            display: grid;
            grid-template-areas:
                "header"
                "nav"
                "content"
                "footer";
            grid-template-rows: auto auto 1fr auto;
            height: 100vh;
            background: #f5f5f5;
        }

        header, nav, footer {
            background: #3e69ad;
            color: white;
            padding: 10px 20px;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            grid-area: header;
        }

        .logo img {
            height: 40px;
        }

        .social a {
            color: white;
            margin-left: 10px;
            text-decoration: none;
        }

        nav {
            display: flex;
            gap: 20px;
            grid-area: nav;
        }

        nav a {
            color: white;
            text-decoration: none;
        }

        .content {
            grid-area: content;
            display: flex;
            gap: 10px;
            padding: 10px;
        }

        aside {
            width: 250px;
            background: #f0f0f0;
            padding: 20px;
        }

        main {
            flex: 1;
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        .box {
            background: white;
            padding: 15px;
            border-radius: 5px;
            flex: 1 1 30%;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        footer {
            grid-area: footer;
            text-align: center;
        }

        @media (max-width: 768px) {
            .content {
                flex-direction: column;
            }  

            .box {
                flex: 1 1 100%;
            }

            aside {
                width: 100%;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">
            <img src="https://www.datwebdigital.com/DWD/wp-content/uploads/2012/06/logo-design.jpg" alt="Logo">
        
        </div>
        <div class="social">
            <a href="#">Facebook</a>
            <a href="#">Twitter</a>
            <a href="#">LinkedIn</a>
        </div>
    </header>
    
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Services</a>
        <a href="#">Contact</a>
    </nav>
    
    <div class="content">
        <aside>
            <h3>Welcome</h3>
            <p>Explore our webpage.</p>
        </aside>
    
        <main>
            <div class="box">
                <h3>Project One</h3>
                <p>This is a short description of project One.</p>
            </div>

            <div class="box">
                <h3>Project Two</h3>
                <p>This is a short description of project Two.</p>
            </div>

            <div class="box">
                <h3>Project Three</h3>
                <p>This is a short description of the project Three.</p>
            </div>
        </main>
    </div>
    
    <footer>
        © 2025 Sushant. All rights reserved.
    </footer>

</body>
</html>
