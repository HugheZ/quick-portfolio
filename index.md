## Portfolio

Below is a complete list of my larger projects, both academic and personal. Only my open-ended apps and research is here, however, so you won't find some more math-heavy applications. Things like my openmp/openmpi - accelerated jaccobi iteration solver, matlab-based decision tree model, and hanabi state-based AI either began with starter functions or are currently assigned as projects at my alma matter, and so they won't be displayed. Feel free to ask me more about them, however.

> Stay tuned for a more personalized website portfolio for my projects, games, and novice voice work, posted once I get my head around 3D fractals. Unless I set my eyes on some work on Boids or a proper synthwave svg library.

---

### [ML Projects](ML_page.md)

I'm new to both machine learning and artificial intelligence, but I've had the opprotunity to apply some basic models, to both interesting and humorous results. This is a small collection of my projects in the area.

---

### [My Games](game_page.md)

A collection of games I've worked on can be found here. All were developed in Unity, and the list contains a mix of platforming and homages.

---

### [Placewise](https://github.com/peterlowrance/placewise)

Placewise is a tool/asset location solution for machine shops. When a manufacturer's employees use expensive tools and parts, lost assets can lead to monetary drain. Placewise is an Angular webapp solution, which allows employees to search through a custom database of tools by category and location. This hierarchy-based structure guides employees from base locations to small cabinets, just like a map. This gives employees a way to find and return parts, decreasing the rate of asset loss.

> Commit logs show my previous commits as an unrecognized user. This was due to a misconfiguration of my local git. It is solved now.

---

### Personal Stuff

#### [Tabletop Helper](https://github.com/HugheZ/Tabletop_Helper)

This is a tabletop assistant designed for Dungeons and Dragons 5th Edition, built using the Python wrapper for QT, PyQt. It allows for character creation while streamlining the process by auto-calculating modifiers and providing roll buttons for skills and weapons. Additionally, the app provides a quick lookup solution by issuing HTTP requests to two D&D REST APIs, as well as a simple initiative tracker for large groups and encounters.

#### [Virtual Tabletop](https://github.com/HugheZ/Virtual_Tabletop)

An in-progress application that virtualizes tabletop board games. With local storage and firebase support, it manages your boards, sizes them by user-reported dimensions, and projects them onto your screen. It is intended to be used with a Raspberry Pi and a secondary TV or large monitor embedded into a coffee table. The result is a table that can take on any board game without having to store boxes and boards while retaining the hands-on feel of moving pieces around. This is primarily useful for tabletop RPGs that rely on 1-inch square tiles, but it could also be useful for modular games like Heroscape, family games like Monopoly, and as a decorative way to spice up your coffee table.

#### [QT Fractals](https://github.com/HugheZ/QT_Fractals)

In the works, this will be a 3D fractal viewer built in QT Quick, QT3D, and OpenGL. Time permitting, I'll also try to port this to HLSL for the Unity engine, though Unity may not handle it well.

3D fractals are a step more complex than traditional 2D fractals. However, 3D surfaces can be made into fractals by some clever mod arithmetic. Similarly, infinite tris and vertices can be rendered using a raytracing substitute known as raymarching. So long as a distance estimation is known, a 3D fractal with any mutation can be rendered entirely in real-time. Big thanks to the [Syntopia](http://blog.hvidtfeldts.net/index.php/2011/06/distance-estimated-3d-fractals-part-i/) blog and [Inigo Quilez](https://www.iquilezles.org/www/index.htm) for help with the maths behind raymarching and 3D fractals.

---

### School Projects

#### [Pong Pow](https://github.com/HugheZ/PongPow)

This was a pong game based in 6502 assembly, an assembly language with only 2 registers, an accumulator, and 8 bit operations. The game makes use of memory-mapped video output to load sprites to the screen by indexing columns and rows on the video memory page. The game implements a power shot feature, game speedup, and pausing.

<img src="images/pong_splash.png?raw=true"/>

#### [Computti Tutti](https://github.com/Ivoah/ComputtiTutti)

Computti Tutti is a simple Java computer-assisted instructor (CAI). The project was developed over the course of a semester with two main sprints, during the first of which I was scrum master. I was in charge of aggregating open-source textbooks and writing more beginner-friendly instructions, writing some boilerplate questions, improving UX through progress bar color changing, and implementing a simple Bayesian classifier through the use of difficulty priors. The app was created in C# using WinForms, the precursor to WPF.

<img src="images/ComputtiTutti_splash.png?raw=true"/>



---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
