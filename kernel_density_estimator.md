# Kernel Density Estimators (KDE)

## Histograms

### Strengths

### Limitations

### Gotchas

## KDE

- Is a composite function made up of one kind of building block referred to as a kernel function.

- The kernel function is evaluated for each datapoint separately, and these partial results are summed to form the KDE

### First Principles

Simplest example. We have one data point, take x = 0.

The most logical approach $exp(-x^2)$

Looks something like this... \

[INSERT GRAPH HERE]

Rescale as area under PDF should be 1. \

\

$K(x) = 1/sqrt(2pi) exp[-(x^2)/2]$

This is our Kernel function and is a valid PDF. Effectively a Gaussian distribution with mean 0 and unit variance

This is our Gaussian kernel.

If we expand it to N datapoints and scale back our PDF, we get a smoother fit of our PDF.

TODO:

- Show a script deriving from first principles using a Guassian Kernel function (like in the towardsdatascience paper)

- Use seaborn as a more polished/modern/faster way of doing it.

- Look into scikit learn and the KernelDensity function that is has. (you can choose different kernels)

## Useful Reading

https://towardsdatascience.com/kernel-density-estimation-explained-step-by-step-7cc5b5bc4517/

https://chriskhanhtran.github.io/_posts/2020-01-13-portfolio-tutorial/
