# Results

The results of this project can be measured using different indicators. The
sections below give an overview of the project using the total complexity of
the function, the number of operations in the function and the number of
assignments.

## Total Complexity

The complexity of the function is measured as the total number of times each
input bit appears in the calculation of an output bit. When all input bits
have been fixed, the total complexity will be reduced to zero.

A reduction of the total complexity may give an indication that the project
if approaching a collision, and if the complexity is reduced to zero without
all input bits being fixed, a collision has indeed been found. However, it can
be expected that if this project will find a collision, the collision will be
found long before the total complexity has been reduced to zero. Also, a large
reduction in the total complexity doesn't guarantee that a collision will be
found: as long as every input bit remains present at least once in the
calculation of an output bit, a collision has not been found.

The performance of the project can be benchmarked against an exponential
reduction of the total complexity, starting from the total complexity for the
situation where no input bit has been fixed, to a value of 1 for 511 input bits
fixed. If a collision can be found, the total complexity will actually be
reduced to 0 for 511 input bits restricted.

| Restrictions  | Target    |  Best Result  | Best Restriction |
|:-------------:|:---------:|:---------:|:------------------:|
|       0       | 1.00×10⁰  | 1.00×10⁰  | |
|       1       | 1.61×10⁻¹ | 3.64×10⁻¹ | F032 |
|       2       | 2.59×10⁻² | 1.87×10⁻² | F031-F032 |
|       3       | 4.17×10⁻³ | 1.40×10⁻² | T029-F031-F032 |
|       4       | 6.71×10⁻⁴ | 9.54×10⁻³ | F029-F030-F031-F032 |

## Number of Operations

## Number of Assignments