# UnumImplementation
f64, f32, and other decimal numbers are used widely in physics simulation. But their use bring unwanted errors, for several reasons.
Listed are some:
computation w/ subnormal numbers : The results might end up too little or too big for representing it.
not knowing whether the floating point number represents the exact number or a number (that cannot be represented) b/c it lies between two numbers
This plan it to implement unums to give at least the most faithful representation of the reals.
The implementation is not really plausible in common programming languages, at least in the most set-theoretical form.
The usual definition is to define an object that inherits operations from interval arithmetic.
On the contrary, a new abstract notion should be in place.
