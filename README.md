# Unum Implementation
f64, f32, and other decimal numbers are used widely in physics simulation. But their use brings unwanted errors, for several reasons.
Listed are some:
Computation w/ subnormal numbers : The results might end up too small or too big for representing it exactly.
Not knowing whether the floating point number represents the exact number or a number (that cannot be represented) b/c it lies between two numbers.
This plan it to implement unums to give at least the most faithful representation of the reals.
The implementation is not really plausible in common programming languages, at least in the most set-theoretical form.
The usual definition is to define an object that inherits operations from interval arithmetic.
On the contrary, a new abstract notion should be in place.
A correct implementation should make use of increase compile-time computation to decrease run-time computation. Such an implementation should be well-versed in calculus.
Interval arithmetic can result in wide intervals. Aspect which is welcome in some cases, where the meaning of the final result is not highly dependent on the final result. The coder should have the choice of whether to use interval arithmetic or to default to a given value within the interval.
Garbage collection is a common cause of high time-complexity. Statical analysis should make that problem disappear. On that note, the choice of language is crutial.

