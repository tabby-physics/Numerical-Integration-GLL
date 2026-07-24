# Numerical Integration with Gauss-Lobatto-Legendre (GLL) Quadrature

A small numerical methods exercise comparing analytical and numerical integration using
Gauss-Lobatto-Legendre (GLL) collocation points and Lagrange interpolation.

## What this does

- Computes GLL collocation points and integration weights for a given polynomial order `N`
- Evaluates a test function `f(x) = x + x^2 + sin(x)` at those points
- Numerically integrates `f(x)` on `[-1, 1]` using GLL quadrature
- Compares the result against the analytical integral
- Builds a Lagrange interpolant through the GLL points and plots it against the original function

## Files

- `Numerical-Integration-GLL.ipynb` — main notebook with the exercise and plots
- `gll.py` — returns GLL collocation points and weights for orders N = 2 to 12
- `lagrange2.py` — evaluates the Lagrange interpolating polynomial at a given point

## Requirements

```
pip install -r requirements.txt
```

## Usage

Open the notebook and run all cells:

```
jupyter notebook Numerical-Integration-GLL.ipynb
```

Try changing `f`, `intf` (the analytical integral), or `N` (the quadrature order) in the
second cell to test different functions and see how quadrature accuracy changes with order.

## Background

This exercise is based on material from a numerical methods for PDEs course covering
finite difference operators, spectral/finite element methods, and GLL quadrature.

## Author

Tabassum Tariq — BS Computational Physics, Centre for High Energy Physics (CHEP),
University of the Punjab, Lahore, Pakistan.
