                setTimeout(displaySlides, 5000); // Change image every 5 seconds
            }

            displaySlides();
        }

        function plusSlides(n, slidesClass) {
            const slidesContainer = document.querySelector(slidesClass + ' .slides');
            const slides = slidesContainer.querySelectorAll('img');
            const totalSlides = slides.length;
            let slideIndex = [...slides].findIndex(slide => slide.style.transform === 'translateX(0%)');

            slideIndex += n;

            if (slideIndex >= totalSlides) {
                slideIndex = 0;
            } else if (slideIndex < 0) {
                slideIndex = totalSlides - 1;
            }

            slidesContainer.style.transform = `translateX(-${slideIndex * 100}%)`;
        }

        showSlides('.slider .slides'); // For the Driveway/Patio Cleaning slider
        showSlides('.gutter-slider .slides'); // For the new Gutter Cleaning slider
    </script>
</body>
</html>
