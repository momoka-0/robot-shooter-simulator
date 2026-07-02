# Robot Shooter Simulator 🥎

## Project Overview 📈
Every year, the global nonprofit robotics youth organization FIRST creates an esports game for high school students around the world to compete in. In the [2026 season game](https://www.youtube.com/watch?v=_fybREErgyM), teams were asked to build robots that could, among other tasks, shoot foam balls (called Fuel) into goals (called Hubs).

For my final project in my Numerical Issues in Scientific Programming class at CCNY, I created a kinematic telemetry system that maps the trajectory of a Fuel into a Hub using interpolation and estimates the Fuel’s total distance traveled using numerical integration.

These predictions are made using a number of numerical approximation methods:

| Trajectory | Total Distance |
| ---------- | -------------- |
| Natural Cubic Spline | Simpson's 1/3 Rule |
| Newton's Divided Difference | Gauss-Legendre Quadrature |
|                      | Gauss-Kronrod Quadrature |

The results of these methods are then compared to each other to determine each method's relative accuracy and to reach a general, acceptable answer.

Tools used:

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

## Set-Up and Installation 🛠️
To clone the repository, run the following command in the terminal in your desired directory:
```
git clone https://github.com/momoka-0/robot-shooter-simulator.git
```

The entirety of this project was implemented using Jupyter Notebooks. To run the .ipynb file, you must have Python packages NumPy, SciPy, Matplotlib, ipympl, and Pillow installed. To install these dependencies, run the command `python -m pip install [package name in lowercase]` (may need to type `python3` instead of `python` if using Python3).

## Next Steps 📋
You may wonder why this project is described as a kinematic telemetry system. This name aptly highlights the fact that the predictions are made based on positional data while making an important distinction that this is not a physics simulator (yet).

Moving forward, I intend to expand on this project to include factors such as force and mass.
