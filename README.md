# libblas-sys

Bindings to BLAS/LAPACK. By default, this crate will build and use a bundled
OpenBLAS. Building this will require a Fortran and C compiler available. For
now, only OpenBLAS is supported, because it is the only actively maintained
BLAS that is multi-threaded and threadsafe by default. Patches to add support
for other threadsafe BLAS/LAPACK variants is welcome.

Two Cargo features are supported:

- `static-blas`: link to blas statically.
- `system-openblas`: don't use the bundled openblas.
