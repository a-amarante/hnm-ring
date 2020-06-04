HNM-Ring Package
===============================
A generator initial conditions tool to handle Minor-Mercury and HNBody packages.
---------------------------------

``HNM-Ring package`` generates the initial conditions of input files for Minor-Mercury [(A. Amarante et al., 2020)](https://github.com/a-amarante/minor-mercury) and HNBody [(Rauch and Hamilton, 2002)](http://janus.astro.umd.edu/HNBody) packages. The user can manipulate several sets of initial condition configurations using ``input.ic`` file. It can handle single star systems, binary, triple, planetary, satellite, coorbital, asteroidal, among others.

The J2-J4-J6 ``Geometric Elements`` computational corrections (Renner and Sicardy, 2006) were also implemented in this version.

How to compile and run
----------------------

The HNM-Ring package is written in ``C programming language``. In the current directory, you should have all files needed to compile and execute the program. Don't hesitate to contact me if any problem arises when trying to use it.
Current package is preconfigured for Linux and Mac OS X users with compile and clean tasks. Use your favorite C compiler, such as ``gcc``, to create an executable. For instance, on Linux or Mac, try:

   ``gcc hnm-ring.c -o hnm-ring -lm``

Now, it should be compiled.  Copy or link the executable wherever you want (wherever your input files are) to run your code using:

   ``./hnm-ring input.ic files.in mer`` (for Minor-Mercury simulations)

   ``./hnm-ring input.ic input.hnb hnbody`` (for HNBody simulations)

Or use the executable file ``hnm-ring`` instead for Linux and Mac OS X compilers:

   First type ``chmod +x hnm-ring`` and after that run your code using one of the commands above.

Disclaimers
------------

* I've fixed all the errors I've found.  If you find a bug, let me know so we can try to fix it.
* Any feedback is appreciated, especially bugs, suggestions, or possible contributions.
* Are you going to publish? Please acknowledge the use of my code in any publication referencing:

   ``Amarante, A., Winter, O. C., Sfair, R. (2020), Stability and Evolution of Fallen Particles Around the Surface of Asteroid (101955) Bennu. JGR Planets.``

* The C source code of this repository is available on reasonable request.

Recent Publications
-------------------

The code was used in the following recent studies:

* Amarante, A., Winter, O. C., Sfair, R. (2020), Stability and Evolution of Fallen Particles Around the Surface of Asteroid (101955) Bennu. JGR Planets.
* G. O. Barbosa, O. C. Winter, A. Amarante, A. Izidoro, R. C. Domingos, E. E. N. Macau (2020), Earth-size planet formation in the habitable zone of circumbinary stars. MNRAS.
* T. S. Moura, O. C. Winter, A. Amarante, R. Sfair, G. Borderes-Motta, G. Valvano (2019), Dynamical environment and surface characteristics of asteroid (16) Psyche. MNRAS.
