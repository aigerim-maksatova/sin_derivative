# sin_derivative
Calculating derivative

import numpy as np
from math import sin
import matplotlib.pyplot as plt

# change in x value
dx = 0.01
def f(x):
    return sin(x) 
sin_x = [x for x in np.arange(0,20,dx)]
sin_y = [f(x) for x in np.arange(0,20,dx)]
# Plot the derivative 
sin_deriv = [(f(x + dx) - f(x)) / dx for x in sin_x]
plt.plot(sin_x, sin_deriv, label="Derivative", linestyle='--')
plt.plot(sin_x, sin_y)
plt.legend(loc="lower right")
# Save the plot as a PNG
plt.savefig('sin_and_derivative_plot.png')

plt.savefig('C:\Users\Uurcp\sin_and_derivative_plot.png')
![image](https://github.com/user-attachments/assets/c73cb6d9-f9f0-42d9-ba35-1bf3ff002796)

![Plot of sin(x) and its Derivative]("C:\Users\Uurcp\sin_and_derivative_plot.png")
