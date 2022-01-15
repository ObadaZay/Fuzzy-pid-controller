# Pendulum Fuzzy controller

This project simulates an inverted pendulum with PID controller and fuzzy controller.

![Simulation](https://github.com/mck-sbs/Pendulum/raw/master/pics/Pendulum.gif)

And it's depending on [This Project](https://github.com/mck-sbs/Pendulum) and the course "Mechatronische Systeme (Mechatronic Systems)", technical college SBS Herzogenaurach-Höchstadt.



## Installation

I prefer to create a new Anaconda virtual environment using this command inside the Anaconda prompt:

`conda create -n pendulum python=3.6.8`

Then activate the environment using:

`conda activate pendulum`

Now you will need to run the following in order to install all the needed packages:

`pip install box2d`

`pip install box2d-py`

`pip install pygame`

`pip install scikit-fuzzy`

## Running the code

Now with everything set up you could run the code, navigate to the folder where the project exists using the same Anaconda prompt with our virtual env `pendulum` activated, this could be done easily using `cd path/to/project`

**Four different control systems included:**

- run Pendulum_PID.py for PID control loop

- run Pendulum_Fuzzy.py for fuzzy control loop

- run Pendulum_Fuzzy_PID.py for combination of fuzzy and PID control loop (runs smoother)

- run Pendulum_Fuzzy_PID_advanced.py for combination of two fuzzy controls to keep the pendulum in the middle

For each system there are some controls could be applied using keyboard

### PID control loop

keyboard commands:

- n: create new world
- m: manual mode
- a: automatic mode

### Fuzzy control loop

fuzzy control loop uses scikit-fuzzy

keyboard commands:

- n: create new world

**Input fuzzy set:**

![input set](https://github.com/mck-sbs/Pendulum/raw/master/pics/input_set.png)

**Output fuzzy set:**

![input set](https://github.com/mck-sbs/Pendulum/raw/master/pics/output_set.png)

**Defuzzification:**

![input set](https://github.com/mck-sbs/Pendulum/raw/master/pics/defuzzification.png)