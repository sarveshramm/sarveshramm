<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sarveshram A - Professional Banner</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Montserrat:wght@400;600;800&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: #fff;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
        }
        
        .banner-container {
            width: 90%;
            max-width: 1200px;
            text-align: center;
            padding: 40px 20px;
            position: relative;
        }
        
        .name {
            font-family: 'Montserrat', sans-serif;
            font-size: 5.5rem;
            font-weight: 800;
            margin-bottom: 20px;
            background: linear-gradient(90deg, #ff8a00, #e52e71, #9b59b6, #3498db);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientShift 8s ease infinite, float 6s ease-in-out infinite;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            letter-spacing: 2px;
        }
        
        .title-container {
            margin: 30px 0;
            height: 80px;
            position: relative;
            overflow: hidden;
        }
        
        .title {
            font-size: 2.2rem;
            font-weight: 300;
            position: absolute;
            width: 100%;
            opacity: 0;
            animation: titleAnimation 12s infinite;
        }
        
        .title:nth-child(1) {
            animation-delay: 0s;
        }
        
        .title:nth-child(2) {
            animation-delay: 4s;
        }
        
        .title:nth-child(3) {
            animation-delay: 8s;
        }
        
        .subtitle {
            font-size: 1.4rem;
            font-weight: 300;
            margin-top: 30px;
            color: #a0aec0;
            animation: fadeIn 2s ease-out;
        }
        
        .decoration {
            position: absolute;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            animation: float 15s infinite linear;
            z-index: -1;
        }
        
        .decoration:nth-child(1) {
            width: 80px;
            height: 80px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
            background: radial-gradient(circle, rgba(255,138,0,0.3) 0%, transparent 70%);
        }
        
        .decoration:nth-child(2) {
            width: 120px;
            height: 120px;
            top: 70%;
            right: 10%;
            animation-delay: -5s;
            background: radial-gradient(circle, rgba(155,89,182,0.3) 0%, transparent 70%);
        }
        
        .decoration:nth-child(3) {
            width: 60px;
            height: 60px;
            bottom: 20%;
            left: 15%;
            animation-delay: -10s;
            background: radial-gradient(circle, rgba(52,152,219,0.3) 0%, transparent 70%);
        }
        
        .decoration:nth-child(4) {
            width: 100px;
            height: 100px;
            top: 20%;
            right: 20%;
            animation-delay: -7s;
            background: radial-gradient(circle, rgba(229,46,113,0.3) 0%, transparent 70%);
        }
        
        .tech-icons {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 40px;
            flex-wrap: wrap;
        }
        
        .tech-icon {
            font-size: 2.5rem;
            color: #cbd5e0;
            transition: all 0.3s ease;
            animation: bounce 2s infinite;
        }
        
        .tech-icon:nth-child(1) { animation-delay: 0.2s; }
        .tech-icon:nth-child(2) { animation-delay: 0.4s; }
        .tech-icon:nth-child(3) { animation-delay: 0.6s; }
        .tech-icon:nth-child(4) { animation-delay: 0.8s; }
        .tech-icon:nth-child(5) { animation-delay: 1s; }
        
        .tech-icon:hover {
            color: #fff;
            transform: scale(1.2);
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        
        @keyframes titleAnimation {
            0% { opacity: 0; transform: translateY(30px); }
            10% { opacity: 1; transform: translateY(0px); }
            30% { opacity: 1; transform: translateY(0px); }
            40% { opacity: 0; transform: translateY(-30px); }
            100% { opacity: 0; transform: translateY(-30px); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            .name {
                font-size: 3.5rem;
            }
            
            .title {
                font-size: 1.8rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .tech-icon {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 480px) {
            .name {
                font-size: 2.5rem;
            }
            
            .title {
                font-size: 1.4rem;
            }
            
            .subtitle {
                font-size: 1rem;
            }
            
            .tech-icon {
                font-size: 1.5rem;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <div class="banner-container">
        <div class="decoration"></div>
        <div class="decoration"></div>
        <div class="decoration"></div>
        <div class="decoration"></div>
        
        <h1 class="name">SARVESHRAM A</h1>
        
        <div class="title-container">
            <h2 class="title">Frontend Developer</h2>
            <h2 class="title">UI/UX Designer</h2>
            <h2 class="title">AI Enthusiast</h2>
        </div>
        
        <p class="subtitle">Crafting digital experiences with code and creativity</p>
        
        <div class="tech-icons">
            <i class="tech-icon fab fa-html5"></i>
            <i class="tech-icon fab fa-css3-alt"></i>
            <i class="tech-icon fab fa-js-square"></i>
            <i class="tech-icon fab fa-react"></i>
            <i class="tech-icon fas fa-brain"></i>
        </div>
    </div>

    <script>
        // Additional animation effects
        document.addEventListener('DOMContentLoaded', function() {
            const nameElement = document.querySelector('.name');
            
            // Add hover effect to name
            nameElement.addEventListener('mouseover', function() {
                this.style.animation = 'gradientShift 3s ease infinite, float 2s ease-in-out infinite';
            });
            
            nameElement.addEventListener('mouseout', function() {
                this.style.animation = 'gradientShift 8s ease infinite, float 6s ease-in-out infinite';
            });
        });
    </script>
</body>
</html>
