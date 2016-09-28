# LAGOS Package Documentation

## Design Philisophy

The design of the LAGOS data package will be guided by these principles:

 * **Package structure and styling will follow best practices for R-data packages.** See the [rOpenSci packaging guide](https://github.com/ropensci/onboarding/blob/master/packaging_guide.md)
 
 * **Internal code will follow a functional programming style.** See the [Motivation Section](http://adv-r.had.co.nz/Functional-programming.html#fp-motivation) of the Functional Programming chapter of the Advanced R book.
 
 * **Data citation information will be displayed prominently.** Definitely make sure that `citation(lagos)` returns a reasonable result. Print citation information on package load?

## Potential Features

 * preloaded database _views_ using ~~`data(LAGOS)`~~ `richfitz/datastorr`
 * API for compiling specific _views_ of LAGOS from the component `txt` files. _Include this info only in a vignette?_
 * filtering by censor codes
 * detection limit handling (imputation?)
 * vignettes to show common workflows (avoid reinventing the wheel as far as analysis and visualization)

## Package Stucture Outline

```
lagos_data()
```

## Legacy code-base

The legacy code-base can be obtained by running the following command in your shell:

```
git clone https://github.com/jsta/LAGOS.git 

cd LAGOS

git checkout 553b0ba3875b29257aab1aaec71d3388070bd3e5
```

## References

[https://help.github.com/articles/distributing-large-binaries/](https://help.github.com/articles/distributing-large-binaries/)

[https://github.com/richfitz/datastorr/blob/master/vignettes/datastorr.Rmd](https://github.com/richfitz/datastorr/blob/master/vignettes/datastorr.Rmd)

[https://github.com/dfalster/baad/releases](https://github.com/dfalster/baad/releases)