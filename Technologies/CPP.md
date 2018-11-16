# C++

# Projects Utilizing C++

## [Inhaler GUI](https://github.com/90301/inhaler_gui)
Debugging multi-robot systems can be a difficult task, doing it in real time is even harder. the Inhaler GUI is designed for
taking many streams in input data and displaying it in an easy to read manner. Utilizing the open source QT graphic engine,
 it's easy to track your ROS (Robot Operating System) based as they go out and explore the world. 
 
 
## Robotics Path Planning and Mapping
[SLAM](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping) (Simultaneous localization and mapping) related problems 
in robotics were the primary focus of the Autonomous Field Robotics Laboratory (AFRL). To that end utilizing Open CV, ROS, 
and a number of other packages we set out to advance the field of autonomous robotics. For the majority of the time I was in the AFRL I
was working on the [Jetyak project](https://afrl.cse.sc.edu/afrl/resources/JetyakWiki/docs/introduction.html)

<img src="https://afrl.cse.sc.edu/afrl/resources/JetyakWiki/_images/jetyak1.jpg">

## C++ Modules for High Performance Code
C++ modules / libraries can be utilized by most languages. If a particular language has performance problems, or low level *bit-flipping* can yield much
faster performance, it is sometimes required to dive into C++. It's rare to need to do this, but one example is in reading large text files, there's an optimization
that you can do in C++, that (as of 2018) is not implemented in any major language that I'm aware of.

In general, this is a *last resort tactic* that should only be used when all other options are exhausted.

# No Simulations?
In general both Java and C# .Net applications perform far better then typical C++ code and even outperforms most heavily optimized C++ code. 
This is due to streaming libraries and Just in Time (JiT) compiling. 