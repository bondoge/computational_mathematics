# Computational Mathematics

This repository contains a collection of computational mathematics projects and seminar notebooks. The projects cover core numerical methods: differentiation, interpolation, integration, series, Fourier analysis, ODEs, boundary value problems, PDEs, finite elements, Monte Carlo methods, and a final visualization-oriented project using FEniCS and Manim.

## Repository Structure

```text
computational_mathematics/
├── 1_numerical_differentiation/
├── 2_interpolation/
├── 3_numerical_integration/
├── 4_series_and_limits/
├── 5_discrete_fourier/
├── 6_Cauchy/
├── 7_boundary/
├── 8_pde/
├── 9_FEM/
├── 10_Monte-Carlo/
└── project_fenics_manim/
```

## Projects

### 1. Numerical Differentiation

Introduces numerical approximation of derivatives using finite-difference formulas. The notebook explores how derivatives can be estimated from discrete function values and how the accuracy depends on the step size and approximation order.

**Main ideas:**
- Forward, backward, and central differences
- Approximation error and convergence
- Numerical instability for very small step sizes

### 2. Interpolation

Covers interpolation methods for reconstructing a function from discrete data points. The project includes seminar materials, an assignment notebook, and input data stored in `data_interp.npz`.

**Main ideas:**
- Polynomial interpolation
- Interpolation error
- Working with sampled numerical data
- Comparing interpolation quality for different grids and methods

### 3. Numerical Integration

Explores numerical quadrature methods for approximating definite integrals when an analytic integral is unavailable or inconvenient.

**Main ideas:**
- Rectangle, trapezoidal, and Simpson-type rules
- Accuracy of quadrature formulas
- Dependence of integration error on grid resolution
- Practical numerical evaluation of integrals

### 4. Series and Limits

Focuses on numerical computation of limits and infinite series. The project demonstrates how finite approximations can be used to study convergence and approximate mathematical quantities.

**Main ideas:**
- Numerical limits
- Partial sums of series
- Convergence behavior
- Accuracy of finite approximations

### 5. Discrete Fourier Transform

Studies the discrete Fourier transform and its use in signal and image processing. The folder contains notebooks, Python scripts, images, and an audio file for practical experiments.

**Main ideas:**
- Discrete Fourier transform
- Frequency-domain representation
- Image and audio processing
- Filtering and reconstruction from Fourier components

**Notable files:**
- `Семинар_+_Задание_5_Дискретный_Фурье.ipynb`
- `rian.py`
- `sound.py`
- Example images: `im1.jpg`, `pov.jpg`, `shrek.jpg`, `zebra.jpg`
- Example audio: `in10.wav`

### 6. Cauchy Problem

Covers numerical solution of initial value problems for ordinary differential equations, also known as Cauchy problems.

**Main ideas:**
- Initial value problems
- Euler-type methods
- Higher-order ODE solvers
- Error accumulation during time integration

**Notable files:**
- `5.1 Семинар - Задача Коши.ipynb`
- `5.1 Задание - Задача Коши.ipynb`

### 7. Boundary Value Problems

Studies boundary value problems, where the solution of a differential equation is constrained by conditions at the boundaries of the domain. The folder also includes a notebook on the Newton–Kantorovich method.

**Main ideas:**
- Boundary value problems for differential equations
- Finite-difference discretization
- Nonlinear equation solving
- Newton–Kantorovich method

**Notable files:**
- `Семинар + Задание 5.2 - Краевая задача.ipynb`
- `Реализация метода Ньютона-Канторовича.ipynb`

### 8. Partial Differential Equations

Introduces numerical methods for partial differential equations using finite differences. The folder includes an HTML animation output.

**Main ideas:**
- PDE discretization
- Finite-difference methods
- Time evolution of PDE solutions
- Visualization of numerical solutions

**Notable files:**
- `Семинар + Задание 5.3 - УРЧП. Метод конечных разностей.ipynb`
- `anim.html`

### 9. Finite Element Method

Introduces the finite element method for solving differential equations by approximating the solution in a finite-dimensional function space.

**Main ideas:**
- Weak formulation of differential equations
- Basis functions and mesh discretization
- Assembly of linear systems
- Numerical solution of boundary value problems using FEM

**Notable file:**
- `Семинар + Задание 5.4 - Finite Element Method.ipynb`

### 10. Monte Carlo Methods

Explores probabilistic numerical methods based on random sampling. The folder includes a general Monte Carlo seminar notebook, a circle-based Monte Carlo example, and a 2D Ising model notebook.

**Main ideas:**
- Random sampling
- Monte Carlo integration
- Estimating geometric quantities probabilistically
- Simulation of physical systems such as the 2D Ising model

**Notable files:**
- `Семинар + Задание 4.3 - Монте Карло.ipynb`
- `monte_carlo_circle.ipynb`
- `Lesson6_2D_Ising.ipynb`

### 11. FEniCS and Manim Project

A final visualization-oriented project combining numerical PDE solving with mathematical animation tools. The notebooks appear to experiment with FEniCS-based finite element simulations and Manim-based visualizations/interactivity.

**Main ideas:**
- Solving PDEs with FEniCS
- Creating mathematical animations with Manim
- Visualizing numerical solutions
- Interactive or animated explanation of computational mathematics concepts

**Notable files:**
- `1.ipynb`
- `2.ipynb`
- `3.ipynb`
- `E05 - interactivity.ipynb`
- `ManimInteractivity.ipynb`
- `media/`

## Requirements

Most projects are written as Jupyter notebooks and use standard scientific Python libraries. A typical environment should include:

```bash
pip install numpy scipy matplotlib pandas jupyter
```

Some projects may require additional packages:

```bash
pip install sympy
pip install manim
```

For the FEniCS project, FEniCS installation is platform-dependent. It is often easiest to run through Docker, Conda, or a dedicated FEniCS environment.

## How to Run

Clone the repository:

```bash
git clone https://github.com/bondoge/computational_mathematics.git
cd computational_mathematics
```

Start Jupyter:

```bash
jupyter notebook
```

Then open the notebook corresponding to the project you want to study.

For Python scripts in the Fourier project, run for example:

```bash
python 5_discrete_fourier/rian.py
python 5_discrete_fourier/sound.py
```

For Manim notebooks or scripts, make sure Manim is installed and configured correctly. Generated animation files are usually saved into a `media/` directory.

## Summary

This repository is a compact course-style collection of computational mathematics projects. It moves from basic numerical approximation methods to differential equation solvers, finite element methods, Monte Carlo simulations, and animated visualization of PDE solutions.
