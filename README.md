<head>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000; /* Change background to black */
            color: #fff; /* Change text color to white */
            box-sizing: border-box;
        }

        header {
            background: linear-gradient(90deg, #000, #333);
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
        }

        .header-container {
            display: flex;
            flex-direction: column; /* Aligns items in a column */
            align-items: center;    /* Centers items horizontally */
        }

        .header-container img {
            height: 300px;
            width: auto;
            display: block; /* Center the logo */
            margin: 0 auto; /* Center the logo */
        }

        nav {
            background-color: #000; /* Ensure nav is black */
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
            color: #000; /* Keep nav links black for contrast */
            font-weight: bold;
            font-size: 1.1em;
            padding: 10px 15px; /* Add padding */
            border-radius: 5px; /* Rounded corners */
            background-color: rgba(255, 215, 0, 0.2); /* Light background for contrast */
            transition: background-color 0.3s ease; /* Smooth transition */
        }

        nav ul li a:hover {
            background-color: rgba(255, 215, 0, 0.5); /* Darker on hover */
        }

        /* Slider styles */
        .slider {
            width: 100%; 
            height: 0; /* Set height to zero */
            padding-top: 100%; /* Maintain a square aspect ratio */
            position: relative;
            overflow: hidden;
            background-color: #000;
            border: 5px solid #FFD700;
        }

        .slides {
            position: absolute;
            top: 0; 
            left: 0; 
            right: 0; 
            bottom: 0; /* Fill the parent */
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%; 
            height: 100%; /* Set height to fill the slider */
            object-fit: contain; /* Change to 'contain' to fit the entire image */
            flex-shrink: 0; 
            display: block;
        }

        .prev,
        .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            width: auto;
            margin-top: -22px;
            padding: 16px;
            color: white;
            font-weight: bold;
            font-size: 18px;
            transition: 0.6s ease;
            border-radius: 0 3px 3px 0;
            user-select: none;
        }

        .next {
            right: 0;
            border-radius: 3px 0 0 3px;
        }

        .prev:hover,
        .next:hover {
            background-color: rgba(255, 215, 0, 0.8); /* Yellow background on hover */
        }

        section {
            padding: 40px 20px; /* Increased padding */
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        section h2 {
            color: #FFD700;
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        section p {
            color: #fff; /* Change section text to white */
        }

        footer {
            background: linear-gradient(90deg, #000, #333);
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        footer h3 {
            margin-bottom: 10px;
            font-size: 1.5em;
        }

        footer p {
            margin: 5px 0;
            font-size: 1.1em;
        }

        footer a {
            color: #FFD700; /* Keep footer links yellow for visibility */
            text-decoration: none; /* Remove underline */
        }

        footer a:hover {
            text-decoration: underline; /* Underline on hover */
        }

        /* Responsive styles */
        @media (max-width: 800px) {
            section {
                padding: 15px;
            }

            footer {
                padding: 15px;
            }

            section h2 {
                font-size: 1.5em; /* Slightly smaller headings */
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
