# Pseudorandom Generators and Statistical Tests

## Project Description

This web project allows you to **generate sequences of pseudorandom numbers** using several classic algorithms and apply **statistical tests** to verify their randomness. It is designed as practical material for the subject **Simulación** at the **Universidad Tecnológica Nacional - Facultad Regional Tucumán (UTN-FRT)**.

## Key Features

- **Pseudorandom number generators:**
  - Additive Congruential Method
  - Mixed Congruential Method
  - Multiplicative Congruential Method
  - Middle Square Method
  - Lehmer Method

- **Implemented statistical tests:**
  - Mean Test
  - Series Test (χ²)
  - Frequency Test (χ²)
  - Runs Test (above and below the mean)
  - Kolmogorov–Smirnov (K–S) Test

- **Quality validation of pseudorandom numbers:**  
  Tools are included to analyze whether the generated numbers are suitable for simulations.

## Technologies Used

- HTML5 + CSS3  
- JavaScript  
- Bootstrap 5.3  

## How to Use

1. Open the main page (index.html).
2. Select a **generator** or a **statistical test**.
3. Fill in the required fields (seed, iterations, critical values, etc.).
4. Click **"Calculate"** or **"Generate"** to run the algorithm.
5. View the results on screen.

## Mathematical Foundation

### Generators

- **Additive Congruential:**
Xₙ = (Xₙ₋₁ + Xₙ₋₂) mod m
- **Mixed Congruential:**
Xₙ₊₁ = (a · Xₙ + c) mod m
- **Multiplicative Congruential:**
Xₙ₊₁ = (a · Xₙ) mod m
- **Middle Square:** Squares the seed and takes the central digits as the new value.
- **Lehmer:** A multiplicative variant that works with bit precision: Xₙ₊₁ = (a · Xₙ) mod m


### Statistical Tests

- **Means:** Evaluates whether the mean of the generated numbers tends to 0.5.  
- **Series:** Analyzes the independence of successive pairs.  
- **Frequency:** Divides values into intervals and compares them with the uniform distribution.  
- **Runs:** Checks randomness in sequences above and below the mean.  
- **Kolmogorov–Smirnov:** Compares the empirical cumulative distribution with the theoretical one.

## Project Status

Completed ✔️  

All generators and tests work correctly and have been validated with sample data.

## File Description

- **index.html**: Home page with a menu linking to generators and tests.  
- **metodoCongruencialAditivo.html**: Interface for the additive congruential generator.  
- **metodoCongruencialMixto.html**: Interface for the mixed congruential generator.  
- **metodoCongruencialMultiplicativo.html**: Interface for the multiplicative congruential generator.  
- **metodoDeLaParteCentralDelCuadrado.html**: Interface for the middle square method.  
- **metodoDeLehmer.html**: Interface for the Lehmer generator.  
- **pruebaDeLosPromedios.html**: Interface for the mean statistical test.  
- **serie.html**: Interface for the series statistical test (χ²).  
- **frecuencia.html**: Interface for the frequency statistical test (χ²).  
- **ks.html**: Interface for the Kolmogorov–Smirnov statistical test.  
- **corrida.html**: Interface for the runs test above and below the mean.  
- **functions/congruencialAditivo.js**: Logic for the additive congruential method.  
- **functions/congruencialMixto.js**: Logic for the mixed congruential method.  
- **functions/congruencialMultiplicativo.js**: Logic for the multiplicative congruential method.  
- **functions/parteCentralCuadrado.js**: Logic for the middle square method.  
- **functions/lehmer.js**: Logic for the Lehmer method.  
- **functions/promedios.js**: Mean statistical test.  
- **functions/serie.js**: Series statistical test (χ²).  
- **functions/frecuencia.js**: Frequency statistical test (χ²).  
- **functions/ks.js**: Kolmogorov–Smirnov statistical test.  
- **functions/corrida.js**: Runs test above and below the mean.
- **css/style.css**: Custom styles for inputs, buttons, and spacing.  
- **public/calculadora-favicon.png**: Project icon visible in the browser tab.

## Access to the Simulator
This project is available online free of charge.
You can access the simulator at the following link:

[Pseudorandom generator and statistical tests](https://pseudorandom-generators-and-tests.netlify.app/)

## Development Team

This project was developed by **Facundo Moya**, a student of **Ingeniería en Sistemas de Información** at **Universidad Tecnológica Nacional – Facultad Regional Tucumán (UTN-FRT)**, as part of the **Simulación** course.

## Code Management

The project development used a simple Git workflow where:

- Single active branch: `master` (now called `main` in many repositories)

## Compatibility and Design

The simulator was designed to be **responsive** thanks to Bootstrap. It works on any device, although medium or large screens are recommended for more comfortable form entry and result viewing.

## How to clone the repository

```bash
git clone https://github.com/facundomoya/pseudorandom-generators-and-tests.git
