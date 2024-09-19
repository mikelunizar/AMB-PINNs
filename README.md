<h1 style="text-align: center; font-family: 'Arial', sans-serif; color: #2c3e50;">
  <strong>UKACM & SEMNI Autumn School: Physics-Enhanced Machine Learning</strong>
</h1>

<p style="text-align: center; font-family: 'Arial', sans-serif; color: #34495e; font-size: 16px;">
  <i>Authors notebook</i>
  </p>
  PhD student <strong>Lucas Tesan</strong>         | ltesan@unizar.es
  </p>
  PhD student <strong>Mikel M. Iparraguirre</strong> | mikel.martinez@unizar.es
</p>

<hr style="border: 1px solid #2c3e50; width: 80%; margin: auto;">

<p style="text-align: center; font-family: 'Arial', sans-serif; color: #34495e; font-size: 18px;">
  This material was created for the UKACM and SEMNI Autumn School 2024, focused on the intersection of physics and machine learning. 

</p>

<p style="text-align: center; font-family: 'Arial', sans-serif; color: #34495e; font-size: 18px;">
  This repository contains two Jupyter notebooks that demonstrate how to solve Ordinary Differential Equations (ODEs) using both <strong>data-driven</strong> methods and <strong>Physics-Informed Neural Networks</strong> (PINNs). Each notebook walks through the problem setup and solution process, clearly highlighting the differences between these two approaches and providing the required basis to build a solid and comprehensive deep learning pipeline.
</p>

## **1. Notebook: An introduction to PINNs**

This notebook provides a detailed walkthrough for solving a Sinusoidal Velocity ODE using both methods. It offers a clear comparison between the data-driven solver and the PINNs approach, covering model setup, training, and result analysis.

- Let's look at the ODE:
<br>
$$\frac{du}{dt} = \cos2\pi t$$
- Initial condition:
<br>
$$u(0) = 1$$
- The exact solution:
<br>
$$u(t) = \frac{1}{2\pi}\sin2\pi t + 1$$


## **2. Notebook: Under damped harmonic oscillator**

Focuses on the Underdamped Harmonic Oscillator problem, showcasing the differences between data-driven and PINNs solutions. It includes a detailed implementation and comparative results.

- Let's look at the ODE:
$$
m \dfrac{d^2 x}{d t^2} + \mu \dfrac{d x}{d t} + kx = 0~,
$$
- Initial conditions in position and velocity
$$
x(0) = 1~~,~~\dfrac{d x}{d t}\bigg|_{t=0} = 0~.
$$

- Because under-damped state:
$$
\delta < \omega_0~,~~~~~\mathrm{with}~~\delta = \dfrac{\mu}{2m}~,~\omega_0 = \sqrt{\dfrac{k}{m}},~~~~ \omega = \sqrt{\omega_0^2 - \delta^2}
$$


This has the following **exact solution**:

$$
 x(t) = e^{-\delta t} \text{cos}(\omega t) + {\delta}\text{sin}(\omega t)
$$
