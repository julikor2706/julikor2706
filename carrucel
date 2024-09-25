
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BMW Store</title>
    <style>
        * {
            padding: 0;
            margin: 0;
            box-sizing: border-box;
        }

        body {
            height: 100vh;
            display: flex;
            flex-direction: column; 
            align-items: center;
            justify-content: center;
            background-image: url('descarga (2).jpg'); 
            background-size: cover; 
            background-position: center;
        }

        h1 {
            margin-bottom: 20px; 
            font-size: 2em; 
            color: #ebe9e9;
            text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.7); 
        } 

        .carousel {
            position: relative;
            width: 600px;
            height: 400px;
            overflow: hidden;
            background-color: rgba(75, 7, 75, 0.8); 
            border-radius: 10px; 
        }

        .slider-section {
            display: none;
            width: 100%;
            height: 100%;
        }

        .slider-section img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .btn-left, .btn-right {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(160, 127, 127, 0.7);
            border: none;
            padding: 10px;
            cursor: pointer;
        }

        .btn-left {
            left: 10px;
        }

        .btn-right {
            right: 10px;
        }
    </style>
</head>
<body>
    <h1 >Tienda BMW</h1>
    <div class="carousel">
        <section class="slider-section" style="display: block;">
            <img src="bm1.jpg" alt="Image 1">
        </section>
        <section class="slider-section">
            <img src="bm3.jpg" alt="Image 2">
        </section>
        <section class="slider-section">
            <img src="bmw 2.jpg" alt="Image 3"> 
        </section>
        <button class="btn-left">&lt;</button>
        <button class="btn-right">&gt;</button>
    </div>

    <script>
        const sections = document.querySelectorAll('.slider-section');
        const btnLeft = document.querySelector('.btn-left');
        const btnRight = document.querySelector('.btn-right');
        let currentIndex = 0;

        function showSlide(index) {
            sections.forEach((section, i) => {
                section.style.display = (i === index) ? 'block' : 'none';
            });
        }

        btnLeft.addEventListener('click', () => {
            currentIndex = (currentIndex === 0) ? sections.length - 1 : currentIndex - 1;
            showSlide(currentIndex);
        });

        btnRight.addEventListener('click', () => {
            currentIndex = (currentIndex === sections.length - 1) ? 0 : currentIndex + 1;
            showSlide(currentIndex);
        });
    </script>
</body>
</html>
