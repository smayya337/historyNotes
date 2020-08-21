# Basic Calculus and 1D Kinematics

## Calculus

### Differentiation

* The average velocity is the change in position over a certain period of time ($\frac{\Delta x}{\Delta t}$)
* Decreasing the duration of that period of time increases the precision of the velocity until you get infinite precision at $\Delta t \approx 0$ (instantaneous velocity)
* Instantaneous velocity is calculated with $v = \frac{dx}{dt}$
* But what if you want to generalize? You can create an equation where plugging in a value gives you the velocity at that point (the derivative)
* Derivative notation:
  * $y(x) \rightarrow y'(x), \frac{dy}{dx}, \dot{y}(x)$
  * Second derivative: $y''(x), \frac{d^2y}{dx^2}, \ddot{y}(x)$
* Taking derivatives
  * Power rule: for an equation $y(x) = ax^b + cx^d$, the derivative will be $y'(x) = abx^{b - 1} + cdx^{d - 1}$
    * If $x(t) = 10t^7 + 5t^3 + 4t + 6$, then $x'(t) = 70t^6 + 15t^2 + 4$
  * Derivative of natural log: $\frac{d}{dx}[\ln{(x)}] = \frac{1}{x}$

### Integration

* The area under a function
* $d = rt$
* Allows you to work in the other direction from differentiation
* Like a derivative, decreasing the change in the $x$-value increases precision
* Notation: $\int f(x)dx$ for an indefinite integral
* Backwards power rule: f $y(x) = 3x^4$, then $\int y(x)dx = \frac{3}{5}x^5 + C$, where $C$ is the constant of differentiation
* Finding area under a certain bound? Use a definite integral
  * For the function $v(t)$ between bounds $t_0$ and $t$ the definite integral is $\int_{t_0}^{t} v(t)dt = x(t)$
  * Make sure to subtract $x(t_0)$ from $x(t)$

## Kinematics

* Recap:
  * Velocity is the time derivative of position ($v = \frac{dx}{dt}$)
  * Acceleration is the time derivative of velocity ($a = \frac{dv}{dt}$)
* Earth's gravitational acceleration is generalized at $g = 9.81 \frac{m}{s^2}$
* Calculating velocity based on acceleration
  * $a = \frac{dv}{dt}$
  * $adt = dv$
  * $\int_0^t adt = \int_{v_0}^v dv$
  * $at|_0^t = v|_{v_0}^v$
  * $at = v - v_0$
  * $v = v_0 + at$
* Calculating position based on velocity
  * $v = \frac{dx}{dt} = v_0 + at$
  * $dx = (v_0 + at)dt$
  * $\int_{x_0}^x dx = \int_0^t (v_0 + at)dt$
  * $x - x_0 = v_0t + \frac{1}{2}at^2$
  * $x = x_0 + v_0t + \frac{1}{2}at^2$
* Calculating the square of velocity from acceleration
  * $a = \frac{dv}{dt} \cdot \frac{dx}{dx}$
  * $a = \frac{dv}{dx} \cdot \frac{dx}{dt}$
  * $a = v \cdot \frac{dv}{dx}$
  * $adx = vdv$
  * $\int_{x_0}^x adx = \int_{v_0}^v vdv$
  * $a(x - x_0) = \frac{1}{2}v^2 - \frac{1}{2}v_0^2$
  * $v^2 = v_0^2 + 2a(x - x_0)$
* Height: $h = \frac{v_0^2}{2g}$

### Relative Motion

* Difference between values
* Relative position: $\vec{x}_{rel} = \vec{x}_B - \vec{x}_A$
* Relative velocity: $\vec{v}_{rel} = \vec{v}_B - \vec{v}_A$
* Relative acceleration: $\vec{a}_{rel} = \vec{a}_B - \vec{a}_A$
