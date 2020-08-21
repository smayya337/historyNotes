# Vectors and Dimensions

## Vectors

* Quantity with direction and magnitude
  * Has a tail and a head
* Direction: where it's pointing
  * 1D: Left/Right
  * 2D: One angle ($\theta$)
  * 3D: Two angles ($\theta$, $\phi$)
* Magnitude: Length/Distance
  * Number + units
  * $\sqrt{x^2+y^2+z^2}$
* Unit Vector: Vector with magnitude of 1
  * Used for direction
  * $\hat{\imath}$, $\hat{\jmath}$, $\hat{k}$ - $x$, $y$, $z$ dimensions respectively

### Vectors vs. Scalars

* Scalars only have a magnitude (no direction)
* Scalars can only be non-negative because negative would imply some sort of direction
* Example: 5 km/hr

### Vector Addition and Subtraction

* Addition
  * Put the tail of the second vector on the head of the first
  * Draw line from tail of first vector to head of second vector
* Subtraction
  * Same as addition, but you have to reverse the direction of the vector doing the subtracting
* Mathematically, you're adding the vector's components
* Commutative when adding
* When given vectors in component form: $a = (a_x, a_y)$ $b = (b_x, b_y)$
  * Add the $x$ and $y$ components
  * $c = (a_x + b_x, a_y + b_y)$
* When given vectors in direction/magnitude form:
  * $a_x = |a|\cos{(\theta)}$ $a_y = |a|\sin{(\theta)}$
  * Do the same for $b$ and add corresponding components
* Convert to direction/magnitude form
  * Direction: $\theta = \arctan{(\frac{a_y}{a_x})}$

### Dot Product

* Scalar vector multiplication
* Result is always a scalar
* Two ways of finding it
  * $A \cdot B = |A||B|\cos{(\theta)}$
  * $A \cdot B = A_xB_x + A_yB_y$
* Commutative
* If the vectors are perpendicular, the dot product is 0
* If the vectors are parallel, the dot product is $|A||B|$
* Finding the angle between vectors given components:
  * $\theta = \arccos{(\frac{A \cdot B}{|A||B|})}$

### Cross Product

* Right hand rule
* Two methods
  * Determinant: $\begin{vmatrix}\hat{\imath} & \hat{\jmath} & \hat{k}\\a_x & a_y & a_z\\b_x & b_y & b_z\end{vmatrix} = A \times B = (A_yB_z - A_zB_y)\hat{\imath} - (A_xB_z - A_zB_x)\hat{\jmath} + (A_xB_y - A_yB_x)\hat{k}$
  * $|A \times B| = |A||B|\sin{(\theta)}$
* Non-commutative, you'll get the opposite vector instead
* If they're perpendicular, the cross product is $|A||B|$
* If they're parallel, the magnitude would be zero

### Vectors: Uses in Physics

* They're used everywhere
* Basic uses
  * Position
  * Displacement
  * Velocity (not to be confused with speed)
  * Acceleration
* Other uses
  * Force
  * Momentum
  * Electric field
* Gives a sense of how different values interact with each other depending on their directions

## Dimensions

* Very simple but crucial concept in physics
* Sense of scale and type of quantities being measured
* Basic dimensions
  * Distance: meter ($m$)
  * Speed meters/second ($\frac{m}{s}$)
  * Acceleration: meters/second squared ($\frac{m}{s^2}$)
* Other cool units
  * Electric field: volts/meter ($\frac{V}{m}$)
  * Magnetic field: Teslas ($T$)
  * Energy: joules ($J$)
  * Always answer a physics question with units!
* Basic SI units:
  * Kilogram ($kg$): mass
  * Meter ($m$): distnace
  * Second ($s$): time
  * Ampere ($A$): current
  * Kelvin ($K$): temperature
  * Mole ($mol$): amount of substance
  * Candela ($cd$): luminous intensity

### Converting Units

* Important in all sciences
* Writing numbers becomes a lot simpler
* Examples
  * Distance from Earth to Sun
  * Speed of light
  * Seconds/minutes/hours
  * Talking to Americans
* Example: day to seconds $\frac{24h}{day} \cdot \frac{60min}{h} \cdot \frac{60s}{min} = \frac{86400s}{day}$
