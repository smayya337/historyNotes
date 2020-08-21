# 2D/3D Kinematics and Uniform Circular Motion

## 2D/3D Kinematics

* Instead of scalars, we're using vectors
* The derivative of a sum is the sum of the derivatives, allowing us to take the derivatives of separate components
* Position vector: $\vec{r} = x\hat{\imath} + y\hat{\jmath} + z\hat{k}$
* Displacement vector: $\Delta\vec{r} = \vec{r_2} - \vec{r_1} = (x_2 - x_1)\hat{\imath} + (y_2 - y_1)\hat{\jmath} + (z_2 - z_1)\hat{k}$
* Average velocity: $\vec{v}_{avg} = \frac{\Delta\vec{r}}{\Delta\vec{t}}$
* Instantaneous velocity: $\vec{v} = \frac{d\vec{r}}{dt} = v_x\hat{\imath} + v_y\hat{\jmath} + v_z\hat{k} = \frac{dx}{dt}\hat{\imath} + \frac{dy}{dt}\hat{\jmath} + \frac{dz}{dt}\hat{k}$
* Average acceleration: $\vec{a}_{avg} = \frac{\Delta\vec{v}}{\Delta\vec{t}}$
* Instantaneous acceleration: $\vec{a} = \frac{d\vec{v}}{dt} = a_x\hat{\imath} + a_y\hat{\jmath} + a_z\hat{k} = \frac{dv_x}{dt}\hat{\imath} + \frac{dv_y}{dt}\hat{\jmath} + \frac{dv_z}{dt}\hat{k}$
* Constant acceleration kinematic equations are still same, there's just a need to work component by component

### Projectile Motion

* A projectile is anything that flies freely through the air (only affected by gravity)
* Air resistance is ignored
* Suppose that we launch a ball with initial speed $v_0$ and angle $\theta$ and we want to know how far it travels before hitting the ground
  * Define unit vectors
    * $\hat{\imath}$ is pointed right (parallel to ground) and $\hat{\jmath}$ is pointed up
  * In vector form, $\vec{v_0} = v_0\cos{(\theta)}\hat{\imath} + v_0\sin{(\theta)}\hat{\jmath}$
  * Acceleration: $\vec{a} = -g\hat{\jmath}$ where $g = 9.81 \frac{m}{s^2}$
  * Y-direction
    * $y = \frac{1}{2}a_yt^2 + v_{0y}t + y_0$
      * $y = y_0$ because the ball returns to the same y-position
      * $a_y = -g$
      * $v_{0y} = v_0\sin{(\theta)}$
    * $0 = \frac{1}{2}a_yt^2 + v_{0y}t$
    * $-\frac{1}{2}a_yt^2 = v_{0y}t$
    * $gt^2 = 2v_0\sin{(\theta)}$
    * $t = 0, \frac{2v_0\sin{(\theta)}}{g}$
  * X-direction
    * $x = \frac{1}{2}a_xt^2 + v_{0x}t + x_0$
      * We're trying to find $x - x_i$
      * $a_x = 0$ because gravity is irrelevant here
      * $v_{0x} = v_0\cos{(\theta)}$
      * $t = \frac{2v_0\sin{(\theta)}}{g}$
    * $x - x_i = v_0\cos{(\theta)} \cdot \frac{2v_0\sin{(\theta)}}{g} = \frac{2v_0^2\sin{(\theta)}\cos{(\theta)}}{g} = \frac{v_0^2\sin{(2\theta)}}{g}$
  * Check with dimensional analysis: $m = \frac{(\frac{m}{s})^2}{\frac{m}{s^2}}$
  * Maximum distance traveled would be at $\theta = 45\deg$

## Uniform Circular Motion

* A particle is traveling at constant speed around a circle
* Although the speed isn't changing, the direction is, so it's technically accelerating the whole time
* Acceleration is always pointed toward the circle's center and has magnitude $a = \frac{v^2}{r}$
* The angular velocity ($\omega$) is the rate at which the angle is changing
  * $\omega = \frac{v}{r}$
* The period ($T$) is the time it takes to complete one revolution around the circle
  * $T = \frac{2\pi}{\omega} = \frac{2\pi r}{v}$

### Derivation of Acceleration

* Any point on the circle with can be characterized with angle $\theta$ between it and the x-axis
* Express the velocity vector $\vec{v}$ in terms of speed $v$ and angle $\theta$: $\vec{v} = -v\sin{(\theta)}\hat{\imath} + v\cos{(\theta)}\hat{\jmath}$
  * $v_x = -v\sin{(\theta)}$ and $v_y = v\cos{(\theta)}$ - switched for similar reasons as an inclined plane
  * $v_x$ is negative because we're assuming it's moving counter-clockwise in this example
* Convert in terms of $x$ and $y$: $\vec{v} = -v\frac{y}{r}\hat{\imath} + v\frac{x}{r}\hat{\jmath} = \frac{v}{r}(-y\hat{\imath} + x\hat{\jmath})$
* Derive: $\vec{a} = \frac{d\vec{v}}{dt} = \frac{v}{r}(-\frac{dy}{dt}\hat{\imath} + \frac{dx}{dt}\hat{\jmath}) = \frac{v}{r}(-v_y\hat{\imath} + v_x\hat{\jmath})$
* Plug values of $v_x$ and $v_y$ back in: $\vec{a} = \frac{v}{r}(-v\cos{(\theta)}\hat{\imath} - v\sin{(\theta)}\hat{\jmath}) = -\frac{v^2}{r}(\cos{(\theta)}\hat{\imath} + \sin{(\theta)}\hat{\jmath})$

## Relative Motion - 2D and 3D

* Suppose two frames, A and B, are moving relative to each other at constant velocity (i.e. $\vec{a}_{AB} = 0)$
* $\vec{v}_{PA} = \vec{v}_{PB} + \vec{v}_{BA}$
  * $\vec{v}_{XY}$ is the velocity of X with respect to Y
* $\vec{a}_{PA} = \vec{a}_{PB}$
