# `ligotimegps`

This module provides a pure-python version of the `LIGOTimeGPS` class, used to represent GPS times (number of seconds elapsed since GPS epoch) with nanoseconds precision.

This module is primarily for use as a drop-in replacement for the 'offical' `lal.LIGOTimeGPS` class (provided by the SWIG-python bindings of [LAL](//wiki.ligo.org/DASWG/LALSuite)) for use on those environments where LAL is not available, or building LAL is unnecessary for the application (e.g. testing).

The code provided here is much slower than the C-implementation provided by LAL, so if you really care about performance, don't use this module.
