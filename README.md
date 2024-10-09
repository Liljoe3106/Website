<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dimension Powerwash</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <style>
        /* CSS for star ratings */
        .star-rating {
            display: flex;
            justify-content: center;
            margin: 10px 0;
        }

        .star {
            color: yellow; /* Yellow stars for branding */
            font-size: 30px;
            cursor: pointer;
        }

        /* Slider styles */
        .slider {
            width: 100%;
            overflow: hidden;
            position: relative;
        }

        .slides {
            display: flex;
            transition: transform 0.5s ease;
        }

        .slide {
            min-width: 100%;
            box-sizing: border-box;
        }

        /* Contact section */
        #contact {
            text-align: center;
            padding: 20px;
            background-color: #f9f9f9;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Dimension Powerwash</h1>
    </header>

    <section id="reviews">
        <h2>Customer Reviews</h2>
        <div class="slider">
            <div class="slides">
                <div class="slide">
                    <p>"Joe did an amazing job on our patio! Highly recommend!"</p>
                    <div class="star-rating">
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                    </div>
                    <p>- Sarah T.</p>
                </div>
                <div class="slide">
                    <p>"Fast, friendly, and affordable. Will use again!"</p>
                    <div class="star-rating">
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                    </div>
                    <p>- Mike R.</p>
                </div>
                <div class="slide">
                    <p>"Excellent service! Our driveway looks brand new!"</p>
                    <div class="star-rating">
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                        <span class="star">&#9733;</span>
                    </div>
                    <p>- Emily W.</p>
                </div>
            </div>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <br />
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Book your free, no obligation quote here!</a>
        <br />
        <br />
        <p>Or Call/Message Joe on:</p>
        <p>Phone: 0114 457 3009 / 07494 503 865</p>
        <p>Also available on Facebook or WhatsApp.</p>
        <br />
        <a href="https://facebook.com/dimensionpowerwash" target="_blank">Follow us on Facebook!</a><br />
    </footer>

    <script>
        $(document).ready(function() {
            let currentIndex = 0;
            const slides = $('.slides');
            const slideCount = $('.slide').length;

            function showSlide(index) {
                const offset = -index * 100; // Move to the correct slide
                slides.css('transform', `translateX(${offset}%)`);
            }

            function nextSlide() {
                currentIndex = (currentIndex + 1) % slideCount;
                showSlide(currentIndex);
            }

            // Change slide every 5 seconds
            setInterval(nextSlide, 5000);

            // Show the first slide initially
            showSlide(currentIndex);
        });
    </script>

</body>
</html>