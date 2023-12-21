# Control of a Two-Pendulum Cart System

This repository contains the modeling, analysis, method description, and implementation (code) of controlling a two-pendulum cart system.

The following have been done as a part of this project.
- System Modeling
- System Linearization
- Controllability Analysis
- LQR Controller Design
- Observability Ananlysis
- Luenberger Observer Design
- LQG Controller Design (using a Kalman-Bucy Filter)

More information about the project, its implementation, and result analysis  can be found in the report, `Report.pdf`.

### Authors

The authors who have developed this project include:
- Lowell Lobo
- Vikram Setty
- Wei-Li Chen

### Code Overview

Apart from the modeling and linearization (that have been done manually using the Euler-Lagrange and small-angle approximation method respectively), all other analysis and implementation have been carried out in MATLAB. These include controllability and observerability checks using rank tests, Luenberger Observer design, and even LQR and LQG controller design. MATLAB'S *sys* and *ode45* functions have been used to simulate system response.

### Code Description

The following list briefly summarizes the functionality of each MATLAB program used in this project.
 - `lqr_v2.mlx`: Checks the controllability of the system and applies the LQR controller to the linearized and nonlinear model
 - `observation.mlx`: Verifies the observability of each output vector representation.
 - `observation_best.mlx`: Creates a state estimator and plots its output response for each observable output vector for the linearized and nonlinear model
 - `observation_script.mlx`: Designs a controller using the previously designed LQR controller and Luenberger observer applied to the linearized and nonlinear model
 - `lqg_script.mlx`: Formulates a LQG controller using the previously designed LQR controller and Luenberger Observer coupled with a Kalman-Bucy Filter applied to the linearized and nonlinear model

### Code Execution

The code files provided in this repository can be executed by adding them into the MATLAB directory and hitting the *Run* command or pressing the *Ctrl* and *Enter* keys simulataneously.

### Video Demosntration

The link to the videos to each of the modules described in the *Code Description* section can be found [here](https://drive.google.com/drive/folders/1cXFvfzNMi8g3eegHmxhW7hi84ukseB2D?usp=sharing).
