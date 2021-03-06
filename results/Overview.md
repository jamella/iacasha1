# Results

The results of this project can be measured using different indicators. The
sections below give an overview of the project using the total complexity of
the function, the number of operations in the function and the number of
assignments.

## Lowest Number of Direct Output Occurrences

The number of direct output occurrences is measured as the number of times an input bit
occurs directly in the last expressions of the calculation of the output bits. Elimination
of an input bit from the last expressions of the calculation of the output bits is the
first step towards a total elimination of the input bit from the calculation.

The performance of the project can be benchmarked against a linear reduction of
the lowest number of direct output occurrences, starting from the lowest number of
direct output occurrences for the situation where no input bit has been fixed, to a
value of 0 for 511 input bits fixed.

Results better than the linear reduction are marked in bold.

| Restrictions | Linear Reduction | Best Reduction | Best Restriction |
|:------------:|:----------------:|:--------------:| ---------------- |
|       0      | 60               | 60             | [Initial Situation](000/000.md) |
|       1      | 60               | (**54**)         | ([E153497](001/e153497.md), [O153497](001/o153497.md)) |
|       2      | 60               | (**54**)         | Many |

![Lowest Number of Direct Output Occurrences](Lowest_Number_of_Direct_Output_Occurrences.png "Lowest Number of Direct Output Occurrences")

## Lowest Number of Direct Occurrences

The number of direct occurrences is measured as the number of times an input bit
occurs directly in an expression in the calculation. If an input bit has been
eliminated from the calculation of the output bits, a collission has been found
as the result of the function will be the same regardless of the value of the
eliminiated input bit. In that case, its number of direct occurrences will have
been reduced to zero.

The performance of the project can be benchmarked against a linear reduction of
the lowest number of direct occurrences, starting from the lowest number of
direct occurrences for the situation where no input bit has been fixed, to a
value of 0 for 511 input bits fixed.

Results better than the linear reduction are marked in bold.

| Restrictions | Linear Reduction | Best Reduction | Best Restriction |
|:------------:|:----------------:|:--------------:| ---------------- |
|       0      | 4,060            | 4,060          | [Initial Situation](000/000.md) |
|       1      | 4,052            | 4,060          | Many             |
|       2      | 4,044            | (4,059)          | ([F511-F512](002/f511_f512.md)) |

![Lowest Number of Direct Occurrences](Lowest_Number_of_Direct_Occurrences.png "Lowest Number of Direct Occurrences")

## Number of Direct Occurrences

The number of direct occurrences is measured as the number of times an input bit
occurs directly in an expression in the calculation. When all input bits have
been fixed, the number of direct occurrences will have been reduced to zero.

A reduction of the number of direct occurrences may give an indication that the
project is approaching a collision, and if the number of direct occurrences is
reduced to zero without all input bits being fixed, a collision has indeed been
found. However, it can be expected that if this project will find a collision,
the collision will be found long before the number of direct occurrences has
been reduced to zero. Also, a large reduction in the number of direct
occurrences doesn't guarantee that a collision will be found: as long as every
input bit remains present at least once in the calculation of an output bit, a
collision has not been found.

The performance of the project can be benchmarked against a linear reduction of
the number of direct occurrences, starting from the number of direct occurrences
for the situation where no input bit has been fixed, to a value of 0 for 511
input bits fixed.

Results better than the linear reduction are marked in bold.

| Restrictions | Linear Reduction | Best Reduction | Best Restriction |
|:------------:|:----------------:|:--------------:| ---------------- |
|       0      | 2,284,331        | 2,284,331      | [Initial Situation](000/000.md) |
|       1      | 2,279,861        | (**2,277,498**)  | ([T256](001/t256.md)) |
|       2      | 2,275,390        | (**2,272,178**)  | ([E069128-T256](002/e069128_t256.md), [O069128-T256](002/o069128_t256.md)) |

![Number of Direct Occurrences](Number_of_Direct_Occurrences.png "Number of Direct Occurrences")

## Complexity of the Least Complex Input Bit

The complexity of an input bit is calculated as the number of times it appears
in the calculation of an output bit. If an input bit has been eliminated from
the calculation of the output bits, a collission has been found as the result
of the function will be the same regardless of the value of the eliminiated
input bit. In that case, its complexity will have been reduced to zero.

The performance of the project can be benchmarked against an exponential
reduction of the complexity of the least complex input bit, starting from the
complexity of the least complex input bit for the situation where no input bit
has been fixed. The goal is to reduce this value to zero for 511 input bits
fixed. Notice however that the measured values will not necessarily relate to
the same input bit: a restriction may reduce the complexity of one input bit
below the complexity of the least complex input bit from the previous round.

Results better than the exponential reduction are marked in bold.

| Restrictions | Exponential Reduction | Best Reduction | Best Restriction |
|:------------:|:---------------------:|:--------------:| ---------------- |
|       0      | 2.62×10³²⁷            | 2.62×10³²⁷     | [Initial Situation](000/000.md) |
|       1      | 5.99×10³²⁶            | 2.62×10³²⁷     | Many             |
|       2      | 1.37×10³²⁶            | 2.62×10³²⁷     | Many             |

![Least Complex Input Bit](Least_Complex_Input_Bit.png "Least Complex Input Bit")

## Total Complexity

The complexity of the function is measured as the total number of times each
input bit appears in the calculation of an output bit. When all input bits
have been fixed, the total complexity will have been reduced to zero.

A reduction of the total complexity may give an indication that the project
is approaching a collision, and if the complexity is reduced to zero without
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

Results better than the exponential reduction are marked in bold.

| Restrictions | Exponential Reduction | Best Reduction | Best Restriction |
|:------------:|:---------------------:|:--------------:| ---------------- |
|       0      | 2.61×10⁴⁰⁵            | 2.61×10⁴⁰⁵     | [Initial Situation](000/000.md) |
|       1      | 4.20×10⁴⁰⁴            | (**1.58×10⁴⁰⁴**) | ([E031032](001/e031032.md)) |
|       2      | 6.76×10⁴⁰³            | (1.56×10⁴⁰⁴)     | ([T002-E031032.md](002/t002_e031032.md)) |

![Total Complexity](Total_Complexity.png "Total Complexity")

## Number of Operations

The number of operations is measured as the number of times the boolean
operators and (“&”), or (“|”) and xor (“^”) appear in the calculation. When all
input bits have been fixed, the number of operators will have been reduced to
zero.

A reduction of the number of operations may give an indication that the project
is approaching a collision, and if the number of operations is reduced to zero
without all input bits being fixed, a collision has indeed been found. However,
it can be expected that if this project will find a collision, the collision
will be found long before the number of operations has been reduced to zero.
Also, a large reduction in the number of operations doesn't guarantee that a
collision will be found: as long as every input bit remains present at least
once in the calculation of an output bit, a collision has not been found.

The performance of the project can be benchmarked against a linear reduction of
the number of operations, starting from the number of operations for the
situation where no input bit has been fixed, to a value of 0 for 511 input bits
fixed.

Results better than the linear reduction are marked in bold.

| Restrictions | Linear Reduction | Best Reduction | Best Restriction |
|:------------:|:----------------:|:--------------:| ---------------- |
|       0      | 25,956,122       | 25,956,122     | [Initial Situation](000/000.md) |
|       1      | 25,905,327       | (**25,901,811**) | ([E031032](001/e031032.md)) |
|       2      | 25,854,532       | (25,892,767)     | ([T002-E031032](002/t002_e031032.md)) |

![Number of Operations](Number_of_Operations.png "Number of Operations")

## Number of Assignments

The number of assignments is measured as the number of local variables used in
the calculation. When all input bits have been fixed, the number of assignments
will have been reduced to zero.

A reduction of the number of assignments may give an indication that the project
is approaching a collision, and if the number of assignments is reduced to zero
without all input bits being fixed, a collision has indeed been found. However,
it can be expected that if this project will find a collision, the collision
will be found long before the number of assignments has been reduced to zero.
Also, a large reduction in the number of assignments doesn't guarantee that a
collision will be found: as long as every input bit remains present at least
once in the calculation of an output bit, a collision has not been found.

The performance of the project can be benchmarked against a linear reduction of
the number of assignments, starting from the number of assignments for the
situation where no input bit has been fixed, to a value of 0 for 511 input bits
fixed.

Results better than the linear reduction are marked in bold.

| Restrictions | Linear Reduction | Best Reduction | Best Restriction |
|:------------:|:----------------:|:--------------:| ---------------- |
|       0      | 47,947           | 47,947         | [Initial Situation](000/000.md) |
|       1      | 47,853           | (24,166)         | ([E031032](001/e031032.md)) |
|       2      | 47,759           | (24,164)         | ([T002-E031032](002/t002_e031032.md), [F002-E031032](002/f002_e031032.md)) |


![Number of Assignments](Number_of_Assignments.png "Number of Assignments")
