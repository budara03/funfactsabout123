# funfactsabout123
GenAI101
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facts About Saturn</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff7e5f, #feb47b);
            transition: background 1s ease;
        }

        header {
            margin-bottom: 20px;
        }

        h1 {
            color: #fff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        main {
            text-align: center;
        }

        #fact-container {
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            margin-bottom: 20px;
            transition: transform 0.5s ease;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            color: #fff;
            background-color: #ff7e5f;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        button:hover {
            background-color: #feb47b;
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <header>
        <h1>Facts About Saturn</h1>
    </header>
    <main>
        <div id="fact-container">
            <p id="fact">Click the button to learn a fact about Saturn!</p>
        </div>
        <button id="random-fact-button">Show Random Fact</button>
    </main>
    <script>
        const facts = [
            "Saturn is the sixth planet from the Sun in our solar system.",
            "It is the second-largest planet in the solar system, after Jupiter.",
            "Saturn is best known for its prominent ring system, which is primarily composed of ice particles, rocky debris, and dust.",
            "The planet is a gas giant, primarily composed of hydrogen and helium.",
            "Saturn has at least 83 moons, with Titan being the largest and the second-largest moon in the solar system.",
            "A day on Saturn lasts about 10.7 hours, but it takes about 29.5 Earth years to orbit the Sun.",
            "Saturn's atmosphere exhibits a banded pattern similar to Jupiter's, but its bands are less distinct.",
            "The planet has a very low density; it is the only planet in the solar system that is less dense than water.",
            "Saturn's magnetic field is weaker than Earth's but has a unique hexagonal storm at its north pole.",
            "The Cassini spacecraft, which orbited Saturn from 2004 to 2017, provided a wealth of information about the planet and its moons."
        ];

        document.getElementById('random-fact-button').addEventListener('click', () => {
            const randomIndex = Math.floor(Math.random() * facts.length);
            const factContainer = document.getElementById('fact-container');
            const factElement = document.getElementById('fact');
            
            // Update the fact text
            factElement.textContent = facts[randomIndex];
            
            // Add animation effect
            factContainer.style.transform = 'scale(1.1)';
            setTimeout(() => {
                factContainer.style.transform = 'scale(1)';
            }, 500);
            
            // Change background gradient
            document.body.style.background = linear-gradient(135deg, #${Math.floor(Math.random()*16777215).toString(16)}, #${Math.floor(Math.random()*16777215).toString(16)});
        });
    </script>
</body>
</html>
