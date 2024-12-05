<html lang="en">
<head>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000;
            color: #fff;
            box-sizing: border-box;
        }
        /* Global heading styles */
        h2, h3 {
            color: #FFD700; /* Yellow color for all section headings */
        }

        .stars {
            color: #FFD700; /* Yellow color */
            font-size: 1.2em; /* Adjust the size if needed */
        }

        header {
            background-color: #000;
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
        }

        .header-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .header-container img {
            height: 300px;
            width: auto;
            display: block;
            margin: 0 auto;
        }

        .header-container p {
            color: #fff;
        }

        nav {
            background-color: #FFD700;
            padding: 10px 0;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            text-decoration: none;
            color: #000;
            font-weight: bold;
            font-size: 1.1em;
            padding: 10px 15px;
            border-radius: 5px;
            background-color: rgba(255, 215, 0, 0.2);
            transition: background-color 0.3s ease;
        }

        nav ul li a:hover {
            background-color: rgba(255, 215, 0, 0.5);
        }

        /* About Us Section */
        #about-us {
            padding: 40px 20px;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        #about-us p strong {
            color: #FFD700; /* Yellow color for keywords */
        }

        /* Review bubble styles */
        .review-bubble {
            background: rgba(255, 215, 0, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 10px auto;
            position: relative;
            max-width: 90%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            height: 275px;
        }

        footer {
            background-color: #000;
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        footer a {
            color: #FFD700;
            text-decoration: underline;
        }

        footer a:hover {
            text-decoration: underline;
        }

        /* Responsive styles */
        @media (max-width: 800px) {
            section, footer {
                padding: 15px;
            }

            section h2 {
                font-size: 1.5em;
            }
        }

        @media (max-width: 600px) {
            nav ul li {
                display: block;
                margin: 5px 0;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo" loading="lazy">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#driveway-patio">Drive & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning">Gutter Cleaning</a></li>
            <li><a href="#roof-cleaning">Roof Cleaning</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="driveway-patio">
        <h2>Drive & Patio Cleaning</h2>
        <ul>
            <li>Remove ingrained dirt, moss, algae, lichen, and black spots.</li>
            <li><strong style="color: #FFD700;">Professional cleaning</strong> for pathways and patios.</li>
        </ul>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <ul>
            <li>Prevent expensive repairs caused by blockages and leaks.</li>
            <li>Clear gutters so that rainwater flows freely.</li>
            <li>Offer full washdown for a <strong style="color: #FFD700;">"like new" appearance</strong>.</li>
        </ul>
    </section>

    <section id="roof-cleaning">
        <h2>Roof Cleaning</h2>
        <ul>
            <li>Remove moss and prevent future growth with <strong style="color: #FFD700;">anti-fungal treatments</strong>.</li>
            <li>Use self-cleaning agents to restore your roof over time.</li>
            <li>Less invasive than pressure washing.</li>
        </ul>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <br />
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <br /><br />
        <p>Call us today for a quote:</p>
        <p>0114 457 3009</p>
        <p>07494503865</p>
        <br />
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a></p>
    </footer>
</body>
</html>
