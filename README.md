# PINN-WyNDA: A Physics Informed Neural Network Method to Discover Mathematical Models of Dynamical Systems from Data

This **PINN-WyNDA** project take inspiration from paper WyNDA https://www.sciencedirect.com/science/article/pii/S2215016124000797?via%3Dihub

Original WyNDA github repo https://github.com/agushasan/discovery

This project consists of two parts:

- [x] Pythonic Implementation of WyNDA Code
- [ ] Implementation of PINNs to WyNDA through extensive study & analysis

**Completed** - Pythonic implementation of WyNDA code

**In Progress** - Implementation of PINNs to WyNDA with extensive study & analysis

## About WyNDA

WyNDA paper introduces a novel method called Wide-Array of Nonlinear Dynamics Approximation 
(WyNDA) for extracting mathematical models of dynamical systems from data. A key advantage 
of this method over existing approaches lies in its suitability for online implementation. Moreover, 
WyNDA stands out by not relying on optimization or machine learning, ensuring computational 
efficiency. The fundamental concept revolves around approximating the unknown function of a 
dynamical system through a diverse set of basis functions that encapsulate the available data. The efficacy of the WyNDA is demonstrated through numerical 
simulations encompassing ***linear systems***, ***nonlinear systems***, and ***control systems***. 


### Linear Systems

The primary aim of this example is to derive a mathematical model for a mass-spring-damper (MSD) system. This system is 
characterized by a first-order linear differential equation encompassing two state variables: position ( 𝑥 ) and velocity ( 𝑣 ). Notably, the 
MSD system is defined by three key parameters, namely the mass ( 𝑚 ), the spring coefficient ( 𝑘 ), and the damper coefficient ( 𝑏 ). To 
initiate this process, we conduct a simulation of MSD system utilizing python matplotlib & numpy to gather pertinent data with 𝑚 = 1 kg, 𝑘 = 84 
N/m, and 𝑏 = 0 . 9 NS/m.

*Captured measurnments of the MSD system's position and velocity data from matplotlib simulation*
<img width="574" height="432" alt="Captured measurements of the MSD system’s position and velocity data from Matplotlib simulation" src="https://github.com/user-attachments/assets/451c41f6-48ae-4899-a173-b41268fdd881" />

*State estimation from measured data*
<img width="554" height="413" alt="State estimation from measured data" src="https://github.com/user-attachments/assets/d256a99d-d1e4-42c7-baac-32761ade5b25" />


### Nonlinear Systems

The objective of this example is to demonstrate the performance of the WyNDA method for nonlinear systems. Specifically, four 
nonlinear mathematical equations are examined: the *Lorenz system*, *Rössler attractor*, *Lotka–Volterra* equations, and *Van der Pol 
oscillator*.

#### Lorentz Systems
The Lorenz system is recognized as a benchmark system in chaotic dynamics due to its remarkable sensitivity to initial conditions 
and the manifestation of the strange attractor phenomenon. In this example, the true value of parameters are: 𝜎= 10 , 𝜌= 28 , and β = 3 . 𝑦1 ( 𝑘 ) , 𝑦2 ( 𝑘 ) , and 𝑦3 ( 𝑘 ) are denoted as the measurements from the sensor system, which were taken every 1 ms. 

*Parameter estimation of the Lorenz system*
<img width="853" height="679" alt="Parameter estimation of the Lorenz system" src="https://github.com/user-attachments/assets/5274746b-bd77-4e9b-9605-1e93b70748b2" />


#### Rössler attractor
The Rössler attractor characterizes a continuous-time dynamical system 
that demonstrates chaotic dynamics, attributed to the fractal properties inherent in the attractor.

*Parameter estimation of the Rössler attractor*
<img width="1003" height="790" alt="Parameter estimation of the Rössler attractor" src="https://github.com/user-attachments/assets/af356e53-9af1-4084-bbc5-be84b267b05f" />


#### Lotka–Volterra
The Lotka-Voltera equations represent a set of first-order nonlinear differential 
equations commonly employed to characterize the dynamics of biological systems involving interaction between two species, one 
acting as a predator and the other as prey.

*Parameter estimation of the Lotka–Volterra equations*
<img width="1203" height="994" alt="Parameter estimation of the Lotka–Volterra equations" src="https://github.com/user-attachments/assets/c8a84fca-e6d2-424e-b1fd-b5a65ab2400f" />


#### Van der Pol oscillator
The Van der Pol oscillator model is an oscillating system with non-linear damping.

*Parameter estimation of the Van der Pol oscillator*
<img width="781" height="589" alt="Parameter estimation of the Van der Pol oscillator" src="https://github.com/user-attachments/assets/f7423663-0ce8-4ef3-aa88-8f532b0105dc" />


### Control Systems
*Parameter estimation with sinusoidal control input*
<img width="990" height="790" alt="Parameter estimation with constant control input" src="https://github.com/user-attachments/assets/96a8a260-d1bc-4038-a9b8-2bcc8c6b568a" />

## Future Directions
The future direction of the following work includes

1. Implementing Physics Informed Neural Network (PINN) into the base **WyNDA** paper for following parameter estimations
2. Extensive analysis of PINN WyNDA model on external dataset for robustness and effectiveness
3. Comparision and analysis for further improvement


## Project Contributors
Contributors of this project are,

1. [Abhinandan Mandal](https://github.com/abhinandan2540)
2. [Ashish Kumar](https://github.com/ashishbringoutthebest-tech)
3. [Abhishek Kumar](https://github.com/abhishek01ds)
4. [Sneha S Karun](https://github.com/snehaskarun22)
5. [J Janasthuthi](https://github.com/jjanasthuthi)


## Acknowledgement
This project is a part of ES526 **Modelling & Simulation** subject. This project is not sponsored by any financial assistance. Contributors of this project are students of **MS Artificial Intelligence & Data Science**. 
Many thanks to **Dr. Purnedu Mishra** and **Dr. Himanshu Jain** for guidance through the project.
