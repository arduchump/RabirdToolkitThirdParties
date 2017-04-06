# RabirdTookitThirdParties

Third party libraries that needs by [RabirdToolkit](https://github.com/starofrainnight/ArduinoRabirdTookitThirdParties) library

## Partial of [Boost](http://www.boost.org) Library (v1.63.0)

Boost provides free peer-reviewed portable C++ source libraries

We only included modules that just implement by pure C++ language without CPU or OS specific stuffs.

They are helpful for library implement.

### Included Modules

* Core
* Algorithm
* Align
* Compatibility
* Concept Check
* Enable If
* MPL
* Preprocessor
* Type Traits
* VMD

### Modules Wants But NOT Included (Their too much dependences)

* Endian
* Metaparse
* TTI
* Type Erasure
* Type Index
* Iterator

### Extract Command
        
    mkdir output
    bcp --unix-lines --boost=. core boost/algorithm/algorithm.hpp boost/algorithm/cxx11 boost/algorithm/cxx14 boost/algorithm/cxx11 align compatibility concept_check  mpl preprocessor type_traits vmd ./output

After generated the partially boost library, just update the boost directory inside the src directory.

### License

Boost Software License, see Boost-LICENSE.

## Protothreads (v1.4)

Protothreads are extremely lightweight stackless threads designed for
severely memory constrained systems such as small embedded systems or
sensor network nodes. Protothreads can be used with or without an
underlying operating system.

### License

BSD-style license, see Protothreads-LICENSE.
        
## Dependences

* StandardCplusplus
