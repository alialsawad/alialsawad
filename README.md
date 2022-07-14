### Hi there 👋

<!--
**alialsawad/alialsawad** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on my Data Science Certification Program
- 🌱 I’m currently learning Data Analysis, Machine Learning and Data Inference
-->


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Portfolio</title>
    <link rel="stylesheet" href="./index.css" />
    <link rel="stylesheet" href="./all.min.css" />
  </head>
  <body>
    <nav>
      <h2 id="logo">Ada Lovelace</h2>
      <ul class="navigation-items">
        <li class="navigation-item"><a href="#about-me">About Me</a></li>
        <li class="navigation-item"><a href="#projects">Projects</a></li>
        <li class="navigation-item"><a href="#skills">Skills</a></li>
        <li class="navigation-item"><a href="/contact.html">Contact</a></li>
      </ul>
    </nav>

    <main>
      <section id="about-me">
        <div class="about-me-container">
          <div class="about-me-text-container">
            <h2>About Me</h2>
            <p>
              Hi! I'm Ada, Countess of Lovelace and am an English mathematician
              and writer, chiefly known for my work on Charles Babbage's
              proposed mechanical general-purpose computer, the Analytical
              Engine.
            </p>
            <p>
              I am one of the first to recognize that machines have applications
              beyond pure calculation, and to have published the first algorithm
              intended to be carried out by such a machine.
            </p>
            <p>
              In my free time I like to read about scientific developments,
              mathematics, and computational mathematics. I also like to take my
              chances of winning big.
            </p>
            <p>
              Fun fact! I've been programing for
              <span id="time-container">0</span> seconds!
            </p>
          </div>
          <img
            src="https://www.biography.com/.image/t_share/MTE4MDAzNDEwODQwOTQ2MTkw/ada-lovelace-20825279-1-402.jpg"
            alt="A photo of Ada Lovelace"
            class="portrait"
          />
        </div>
      </section>

      <section id="projects">
        <h2>Projects</h2>
        <details class="project">
          <summary class="project-title">
            <h3>The first computer program</h3>
          </summary>
          <img
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/Diagram_for_the_computation_of_Bernoulli_numbers.jpg/220px-Diagram_for_the_computation_of_Bernoulli_numbers.jpg"
            alt="Lovelace's diagram from note G, the first published computer
          algorithm"
            class="project-image"
          />
          <p class="project-description">
            The world's first computer program for computing Bernoulli numbers.
          </p>
        </details>
        <details class="project">
          <summary class="project-title">
            <h3>The Analytical Engine</h3>
          </summary>
          <img
            src="https://images2.minutemediacdn.com/image/upload/c_fit,f_auto,fl_lossy,q_auto,w_728/v1555925585/shape/mentalfloss/analyticalmachine_babbage_london.jpg?itok=5vRTwQjb"
            alt="An original model of part of the Analytical Engine"
            class="project-image"
          />
          <p class="project-description">
            I helped Charles Babbage on topics ranging from math to computation
            that helped the development of the Analytical Engine.
          </p>
        </details>
        <details class="project">
          <summary class="project-title">
            <h3>The Ada programming language</h3>
          </summary>
          <img
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Ada_Mascot_with_slogan.svg/220px-Ada_Mascot_with_slogan.svg.png"
            alt='Ada mascot, a black and cobalt blue hummingbird, flying above the
          slogan "Time-tested, safe and secure"'
            class="project-image"
          />
          <p class="project-description">
            My work inspired the United States Department of Defense to name
            their new programming language after me.
          </p>
        </details>
      </section>

      <section id="skills">
        <h2>Skills</h2>
        <div id="skills-container">
          <i class="fab fa-html5"></i>
          <i class="fab fa-css3-alt"></i>
          <i class="fab fa-js"></i>
          <i class="fab fa-react"></i>
          <i class="fab fa-aws"></i>
          <i class="fab fa-sketch"></i>
          <i class="fab fa-figma"></i>
          <i class="fab fa-git"></i>
          <i class="fab fa-chrome"></i>
          <i class="fas fa-terminal"></i>
          <i class="fas fa-universal-access"></i>
          <i class="fab fa-npm"></i>
          <i class="fab fa-node"></i>
          <i class="fab fa-github"></i>
        </div>
      </section>
    </main>

    <footer>Made with <span class="heart">♥</span> in London</footer>
  </body>
  <script>
    const timeContainer = document.getElementById("time-container");
    const BIRTH_DAY = "12-10-1815";
    const BIRTH_DAY_DATE = new Date(BIRTH_DAY);
    const intlNumberFormatter = new Intl.NumberFormat("en-US");

    setInterval(() => {
      const now = new Date();
      const difference = Math.floor(
        (now.getTime() - BIRTH_DAY_DATE.getTime()) / 1000
      );

      timeContainer.innerText = intlNumberFormatter.format(difference);
    }, 1000);
  </script>
</html>

