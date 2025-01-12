[WIP]

# My (more notable) Projects

**Table of Contents** 
- [Game Scripting Engine](#gamescriptingengine)
- [Raytracing](#raytracing)  
- [SFML based space shooter game](#spaceranger) 
- [SFML based particle system](#sfml_particles)
- [Random mini-projects](#collection)

## GameScriptingEngine
Automation/scripting engine to simplify repetetive actions (goodbye RSI just to play some games...). Currently, under development. ![image](Images\game_scripting_engine.png)
Features:
- an AutoClicker,
- a basic scripting engine (click, mouse move, send keys, sleeps, delays, loop inner script), with parsing to and
from file,
- a monitor pixel reader,
- a template searcher (openCV),
- a snipping tool (similar to windows+shift+s), with auto updates of the image (used by the monitor pixel reader,
and template searcher for optimization),
- a console output widget,
- hotkeys system,

Scripts can be created via builder pattern, like so:
```c++
SyncScriptBuilder()
                   .send(Keyboard::KEY::I)
                   .press(position, 50)
                   .send(Keyboard::KEY::I)
                   .click(nest_pos)
                   .click(animal_pos)
                   .setStepDelay(0)
                   .loop(new Script(SyncScriptBuilder().click(breed_pos).click(scrap).build()), 10)
                   .setStepDelay(delay.count())
                   .build()
```




## Raytracing
The initial version based on ***The Ray Tracer Challenge*** book by ***Jamis Buck*** implemented in C# can be found [here](https://kagonkhan.github.io/RayTracingCS/). Features multiple light sources, transparency, reflectivity, materials, patterns, and more!. A vector/matrix basic library has been implemented as well.
![Image](https://raw.githubusercontent.com/KagonKhan/RayTracingCS/refs/heads/master/examples/8.png)

Later, the project was moved to C++ ([here](https://github.com/KagonKhan/CompileTimeRayTracer)) in order to achieve compile-time raytracing. Successful (?) but not really worth it. A lot of fiddling with compiler settings to allow larger stack sizes, longer tracing times, and smaller max resolutions.

And recently, I implemented a version utilizing [DearImGui](https://github.com/ocornut/imgui) found [here](https://github.com/KagonKhan/RayTracerV2). The implementation is fairly basic, but it's real-time with an object editor/picker and an interactable camera. Work on hold, until I go through the Physically Based Rendering book.
![Image](Images\real-time_raytracing.png)





## SpaceRanger
More on the project can be found [here](https://kagonkhan.github.io/SpaceRanger/). A 2D space shooting game, utilizing the SFML library. The game style choice was inspired by the Space Invaders title. Many game techniques (natural movement, tracking systems, collision detection) and design patterns (singletons, commands, inheritance trees, flyweights, states, factories) have been utilized. Additionally, a GUI system has been implemented.
![Image](https://raw.githubusercontent.com/KagonKhan/SpaceRanger/master/examples/ex1.png)


## SFML_Particles
A very basic particle system, will be finished... soon <sup>tm</sup>. Project [here](https://github.com/KagonKhan/SFML_particles).
<p float="left">
  <img src="Images\particles_1.png" width="49%" />
  <img src="Images\particles_2.png" width="49%" /> 
</p>






## Collection
- [AHK](#ahk)  
- [Algorithms](#algorithms) 
- [Audio manipulation](#audio-manipulation)
- [OpenGL](#opengl)
- [RegEx](#regex)
- [Web applications](#web-applications)
- [Mini games](#mini-games)


### AutoHotkey
A [collection](https://github.com/KagonKhan/RepoLection/tree/main/AHK) of useful scripts at the time. Currently `mousePos` finder and `image` finder. Can be used for an auto clicker finding images on screen.


### Algorithms
A [collection](https://github.com/KagonKhan/RepoLection/tree/main/Algorithms) of code files related to algorithmics. Data structures, graphs, sorting,  challenges, etc...



### Audio manipulation
A [Library](https://github.com/KagonKhan/RepoLection/tree/main/AudioManipulationProject/AudioManipulation) for generating waves (sine, triangle, saw, rectangular), notes, applying envelopes, adding echoes, and filters!


### OpenGL
SDL version tutorial and following the OpenGL [book](https://learnopengl.com/) found [here](https://github.com/KagonKhan/RepoLection/tree/main/OpenGL)
TODO: Add results


### Regular Expressions
Space for learning RegEx (good regex library in cpp when?)


### Web Applications
Python based web apps. Django, Django with flavor (bootstrap), and Flask apps.
TODO: Add results, more description


### Mini Games
A [collection](https://github.com/KagonKhan/RepoLection/tree/main/unfinished-games) of either smaller, unfinished, or WIP games.
-  Tetris-dragging-puzzle game.
-  Checkers.
-  Doodle Jump.
-  Flabby birb (PyGame).
-  IdleOn mining minigame (PyGame).
-  SFML based RPG.
-  SFML based GUI system.


<!--
[comment]: <> (
**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/KagonKhan/KagonKhan/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

```
)



## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/KagonKhan/KagonKhan/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.)



-->
