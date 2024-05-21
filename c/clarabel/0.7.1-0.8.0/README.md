# Comparing `tmp/clarabel-0.7.1.tar.gz` & `tmp/clarabel-0.8.0.tar.gz`

## Comparing `clarabel-0.7.1.tar` & `clarabel-0.8.0.tar`

### file list

```diff
@@ -1,156 +1,175 @@
--rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 clarabel-0.7.1/Cargo.toml
--rw-r--r--   0     1001      127      237 2024-03-01 23:13:49.000000 clarabel-0.7.1/.cargo/config.toml
--rw-r--r--   0     1001      127      760 2024-03-01 23:13:49.000000 clarabel-0.7.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     5191 2024-03-01 23:13:49.000000 clarabel-0.7.1/.github/workflows/pypi.yaml
--rw-r--r--   0     1001      127     4948 2024-03-01 23:13:49.000000 clarabel-0.7.1/.github/workflows/testpypi.yaml
--rw-r--r--   0     1001      127       82 2024-03-01 23:13:49.000000 clarabel-0.7.1/.gitignore
--rw-r--r--   0     1001      127     6310 2024-03-01 23:13:49.000000 clarabel-0.7.1/CHANGELOG.md
--rw-r--r--   0     1001      127    38660 2024-03-01 23:14:01.000000 clarabel-0.7.1/Cargo.lock
--rw-r--r--   0     1001      127    10779 2024-03-01 23:13:49.000000 clarabel-0.7.1/LICENSE.md
--rw-r--r--   0     1001      127     4013 2024-03-01 23:13:49.000000 clarabel-0.7.1/README.md
--rw-r--r--   0     1001      127      430 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_box.py
--rw-r--r--   0     1001      127      613 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_expcone.py
--rw-r--r--   0     1001      127      689 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_powcone.py
--rw-r--r--   0     1001      127      891 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_qp.py
--rw-r--r--   0     1001      127      710 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_sdp.py
--rw-r--r--   0     1001      127      650 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/python/example_socp.py
--rw-r--r--   0     1001      127      807 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_box.rs
--rw-r--r--   0     1001      127      711 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_expcone.rs
--rw-r--r--   0     1001      127      985 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_lp.rs
--rw-r--r--   0     1001      127     1141 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_powcone.rs
--rw-r--r--   0     1001      127     1756 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_qp.rs
--rw-r--r--   0     1001      127      830 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_sdp.rs
--rw-r--r--   0     1001      127      598 2024-03-01 23:13:49.000000 clarabel-0.7.1/examples/rust/example_socp.rs
--rw-r--r--   0     1001      127      696 2024-03-01 23:13:49.000000 clarabel-0.7.1/html/rustdocs-header.html
--rw-r--r--   0     1001      127      152 2024-03-01 23:13:49.000000 clarabel-0.7.1/python/clarabel/__init__.py
--rw-r--r--   0     1001      127       38 2024-03-01 23:13:49.000000 clarabel-0.7.1/rustfmt.toml
--rw-r--r--   0     1001      127      348 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/adjoint.rs
--rw-r--r--   0     1001      127     1998 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/csc/block_concatenate.rs
--rw-r--r--   0     1001      127    16175 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/csc/core.rs
--rw-r--r--   0     1001      127     8649 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/csc/matrix_math.rs
--rw-r--r--   0     1001      127      183 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/csc/mod.rs
--rw-r--r--   0     1001      127     9473 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/csc/utils.rs
--rw-r--r--   0     1001      127    10721 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/blas.rs
--rw-r--r--   0     1001      127     1882 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/blaslike_traits.rs
--rw-r--r--   0     1001      127     1520 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/block_concatenate.rs
--rw-r--r--   0     1001      127     2547 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/cholesky.rs
--rw-r--r--   0     1001      127     7958 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/core.rs
--rw-r--r--   0     1001      127     2250 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/gemm.rs
--rw-r--r--   0     1001      127     1980 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/gemv.rs
--rw-r--r--   0     1001      127     2218 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/kron.rs
--rw-r--r--   0     1001      127     4633 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/matrix_math.rs
--rw-r--r--   0     1001      127      396 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/mod.rs
--rw-r--r--   0     1001      127     4384 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/svd.rs
--rw-r--r--   0     1001      127     4547 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/syevr.rs
--rw-r--r--   0     1001      127     1060 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/symv.rs
--rw-r--r--   0     1001      127     1649 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/syr2k.rs
--rw-r--r--   0     1001      127     1738 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/dense/syrk.rs
--rw-r--r--   0     1001      127     6914 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/densesym3x3/mod.rs
--rw-r--r--   0     1001      127     1030 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/error_types.rs
--rw-r--r--   0     1001      127     3237 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/floats.rs
--rw-r--r--   0     1001      127     6572 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/math_traits.rs
--rw-r--r--   0     1001      127     1306 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/matrix_traits.rs
--rw-r--r--   0     1001      127     1959 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/matrix_types.rs
--rw-r--r--   0     1001      127     1318 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/mod.rs
--rw-r--r--   0     1001      127      344 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/reshaped.rs
--rw-r--r--   0     1001      127      753 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/scalarmath.rs
--rw-r--r--   0     1001      127      352 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/symmetric.rs
--rw-r--r--   0     1001      127     9439 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/tests/matrix.rs
--rw-r--r--   0     1001      127       24 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/tests/mod.rs
--rw-r--r--   0     1001      127     3744 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/tests/vector.rs
--rw-r--r--   0     1001      127     5139 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/algebra/vecmath.rs
--rw-r--r--   0     1001      127       14 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/.gitignore
--rw-r--r--   0     1001      127      418 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/Project.toml
--rw-r--r--   0     1001      127     1442 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/src/ClarabelRs.jl
--rw-r--r--   0     1001      127      218 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/src/MOI_wrapper.jl
--rw-r--r--   0     1001      127     4763 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/src/interface.jl
--rw-r--r--   0     1001      127     2570 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/src/types.jl
--rw-r--r--   0     1001      127     3125 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl
--rw-r--r--   0     1001      127      955 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/test/test_jump.jl
--rw-r--r--   0     1001      127      238 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/ClarabelRs/test/test_problem_depot.jl
--rw-r--r--   0     1001      127      736 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/README.md
--rw-r--r--   0     1001      127     4032 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/interface.rs
--rw-r--r--   0     1001      127       48 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/mod.rs
--rw-r--r--   0     1001      127     3572 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/julia/types.rs
--rw-r--r--   0     1001      127     3093 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/lib.rs
--rw-r--r--   0     1001      127     1463 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      685 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/.gitignore
--rw-r--r--   0     1001      127     5633 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/cones_py.rs
--rw-r--r--   0     1001      127     1163 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/cscmatrix_py.rs
--rw-r--r--   0     1001      127    14286 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/impl_default_py.rs
--rw-r--r--   0     1001      127     2588 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/io.rs
--rw-r--r--   0     1001      127      873 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/mod.rs
--rw-r--r--   0     1001      127     1765 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/module_py.rs
--rw-r--r--   0     1001      127      871 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/blas_loader.rs
--rw-r--r--   0     1001      127     3695 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/blas_types.rs
--rw-r--r--   0     1001      127     4962 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/blas_wrappers.rs
--rw-r--r--   0     1001      127      705 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/lapack_loader.rs
--rw-r--r--   0     1001      127     2891 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/lapack_types.rs
--rw-r--r--   0     1001      127     4692 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/lapack_wrappers.rs
--rw-r--r--   0     1001      127     1186 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/python/pyblas/mod.rs
--rw-r--r--   0     1001      127      117 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/qdldl/mod.rs
--rw-r--r--   0     1001      127    25632 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/qdldl/qdldl.rs
--rw-r--r--   0     1001      127     8608 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/qdldl/test.rs
--rw-r--r--   0     1001      127    11066 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/compositecone.rs
--rw-r--r--   0     1001      127    13340 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/expcone.rs
--rw-r--r--   0     1001      127    13721 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/genpowcone.rs
--rw-r--r--   0     1001      127     5367 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/mod.rs
--rw-r--r--   0     1001      127     5798 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/nonnegativecone.rs
--rw-r--r--   0     1001      127     6478 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/nonsymmetric_common.rs
--rw-r--r--   0     1001      127    14599 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/powcone.rs
--rw-r--r--   0     1001      127    14615 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/psdtrianglecone.rs
--rw-r--r--   0     1001      127    15307 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/socone.rs
--rw-r--r--   0     1001      127     7481 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/supportedcone.rs
--rw-r--r--   0     1001      127     3257 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/symmetric_common.rs
--rw-r--r--   0     1001      127     2912 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/cones/zerocone.rs
--rw-r--r--   0     1001      127       35 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/mod.rs
--rw-r--r--   0     1001      127    11788 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
--rw-r--r--   0     1001      127    12374 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
--rw-r--r--   0     1001      127     8547 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
--rw-r--r--   0     1001      127       15 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
--rw-r--r--   0     1001      127     2743 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
--rw-r--r--   0     1001      127      688 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/mod.rs
--rw-r--r--   0     1001      127      517 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/kktsolvers/mod.rs
--rw-r--r--   0     1001      127      402 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/mod.rs
--rw-r--r--   0     1001      127      293 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/settings.rs
--rw-r--r--   0     1001      127    20434 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/solver.rs
--rw-r--r--   0     1001      127     7334 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/core/traits.rs
--rw-r--r--   0     1001      127     8443 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/data_updating.rs
--rw-r--r--   0     1001      127      953 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/equilibration.rs
--rw-r--r--   0     1001      127    11341 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/info.rs
--rw-r--r--   0     1001      127     9289 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/info_print.rs
--rw-r--r--   0     1001      127     8358 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/kktsystem.rs
--rw-r--r--   0     1001      127      615 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/mod.rs
--rw-r--r--   0     1001      127     4168 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/presolver.rs
--rw-r--r--   0     1001      127     7114 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/problemdata.rs
--rw-r--r--   0     1001      127     2984 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/residuals.rs
--rw-r--r--   0     1001      127     3957 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/settings.rs
--rw-r--r--   0     1001      127     3359 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/solution.rs
--rw-r--r--   0     1001      127     3225 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/solver.rs
--rw-r--r--   0     1001      127     7639 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/default/variables.rs
--rw-r--r--   0     1001      127       77 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/implementations/mod.rs
--rw-r--r--   0     1001      127     1898 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/mod.rs
--rw-r--r--   0     1001      127      832 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/tests/cones.rs
--rw-r--r--   0     1001      127       11 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/tests/mod.rs
--rw-r--r--   0     1001      127      761 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/utils/atomic.rs
--rw-r--r--   0     1001      127     1327 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/utils/infbounds.rs
--rw-r--r--   0     1001      127       94 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/solver/utils/mod.rs
--rw-r--r--   0     1001      127      367 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/stdio/mod.rs
--rw-r--r--   0     1001      127      109 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/timers/mod.rs
--rw-r--r--   0     1001      127     5066 2024-03-01 23:13:49.000000 clarabel-0.7.1/src/timers/timers.rs
--rw-r--r--   0     1001      127     2352 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/api_dimension_checks.rs
--rw-r--r--   0     1001      127     2328 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_eq_constrained.rs
--rw-r--r--   0     1001      127     2807 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_expcone.rs
--rw-r--r--   0     1001      127     1439 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_genpowcone.rs
--rw-r--r--   0     1001      127     2605 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_lp.rs
--rw-r--r--   0     1001      127     1382 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_powcone.rs
--rw-r--r--   0     1001      127     4426 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_qp.rs
--rw-r--r--   0     1001      127     2493 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_sdp.rs
--rw-r--r--   0     1001      127     2419 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_socp.rs
--rw-r--r--   0     1001      127      989 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/basic_unconstrained.rs
--rw-r--r--   0     1001      127     9287 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/data_updating.rs
--rw-r--r--   0     1001      127     2608 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/equilibration_bounds.rs
--rw-r--r--   0     1001      127     1126 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/mixed_conic.rs
--rw-r--r--   0     1001      127     2408 2024-03-01 23:13:49.000000 clarabel-0.7.1/tests/presolve.rs
--rw-r--r--   0     1001      127      290 2024-03-01 23:13:49.000000 clarabel-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4587 1970-01-01 00:00:00.000000 clarabel-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 clarabel-0.8.0/Cargo.toml
+-rw-r--r--   0     1001      127      237 2024-05-21 12:09:13.000000 clarabel-0.8.0/.cargo/config.toml
+-rw-r--r--   0     1001      127      496 2024-05-21 12:09:13.000000 clarabel-0.8.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127      760 2024-05-21 12:09:13.000000 clarabel-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     5159 2024-05-21 12:09:13.000000 clarabel-0.8.0/.github/workflows/pypi.yaml
+-rw-r--r--   0     1001      127     4948 2024-05-21 12:09:13.000000 clarabel-0.8.0/.github/workflows/testpypi.yaml
+-rw-r--r--   0     1001      127       82 2024-05-21 12:09:13.000000 clarabel-0.8.0/.gitignore
+-rw-r--r--   0     1001      127     7173 2024-05-21 12:09:13.000000 clarabel-0.8.0/CHANGELOG.md
+-rw-r--r--   0     1001      127    49028 2024-05-21 12:09:26.000000 clarabel-0.8.0/Cargo.lock
+-rw-r--r--   0     1001      127    10779 2024-05-21 12:09:13.000000 clarabel-0.8.0/LICENSE.md
+-rw-r--r--   0     1001      127     3896 2024-05-21 12:09:13.000000 clarabel-0.8.0/README.md
+-rw-r--r--   0     1001      127      430 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_box.py
+-rw-r--r--   0     1001      127      613 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_expcone.py
+-rw-r--r--   0     1001      127      689 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_powcone.py
+-rw-r--r--   0     1001      127      891 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_qp.py
+-rw-r--r--   0     1001      127      710 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_sdp.py
+-rw-r--r--   0     1001      127      650 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/python/example_socp.py
+-rw-r--r--   0     1001      127      807 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_box.rs
+-rw-r--r--   0     1001      127      711 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_expcone.rs
+-rw-r--r--   0     1001      127      985 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_lp.rs
+-rw-r--r--   0     1001      127     1141 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_powcone.rs
+-rw-r--r--   0     1001      127     1756 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_qp.rs
+-rw-r--r--   0     1001      127      830 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_sdp.rs
+-rw-r--r--   0     1001      127      598 2024-05-21 12:09:13.000000 clarabel-0.8.0/examples/rust/example_socp.rs
+-rw-r--r--   0     1001      127      696 2024-05-21 12:09:13.000000 clarabel-0.8.0/html/rustdocs-header.html
+-rw-r--r--   0     1001      127      152 2024-05-21 12:09:13.000000 clarabel-0.8.0/python/clarabel/__init__.py
+-rw-r--r--   0     1001      127       38 2024-05-21 12:09:13.000000 clarabel-0.8.0/rustfmt.toml
+-rw-r--r--   0     1001      127     6019 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/csc/block_concatenate.rs
+-rw-r--r--   0     1001      127    24016 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/csc/core.rs
+-rw-r--r--   0     1001      127     9073 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/csc/matrix_math.rs
+-rw-r--r--   0     1001      127      111 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/csc/mod.rs
+-rw-r--r--   0     1001      127     9917 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/csc/utils.rs
+-rw-r--r--   0     1001      127     3925 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/cholesky.rs
+-rw-r--r--   0     1001      127     2210 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/gemm.rs
+-rw-r--r--   0     1001      127     2050 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/gemv.rs
+-rw-r--r--   0     1001      127     1575 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/lu.rs
+-rw-r--r--   0     1001      127      237 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/mod.rs
+-rw-r--r--   0     1001      127     7152 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/svd.rs
+-rw-r--r--   0     1001      127     4690 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/syevr.rs
+-rw-r--r--   0     1001      127     1060 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/symv.rs
+-rw-r--r--   0     1001      127     1710 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/syr2k.rs
+-rw-r--r--   0     1001      127     1727 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/syrk.rs
+-rw-r--r--   0     1001      127    12290 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blas/traits.rs
+-rw-r--r--   0     1001      127     3552 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/blaslike_traits.rs
+-rw-r--r--   0     1001      127     3533 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/block_concatenate.rs
+-rw-r--r--   0     1001      127      687 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/borrowed.rs
+-rw-r--r--   0     1001      127     7476 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/core.rs
+-rw-r--r--   0     1001      127     2148 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/kron.rs
+-rw-r--r--   0     1001      127     7111 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/matrix_math.rs
+-rw-r--r--   0     1001      127      250 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/mod.rs
+-rw-r--r--   0     1001      127     4778 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/dense/types.rs
+-rw-r--r--   0     1001      127     6895 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/densesym3x3/mod.rs
+-rw-r--r--   0     1001      127     1251 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/error_types.rs
+-rw-r--r--   0     1001      127     3774 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/floats.rs
+-rw-r--r--   0     1001      127     6446 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/math_traits.rs
+-rw-r--r--   0     1001      127     2423 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/matrix_traits.rs
+-rw-r--r--   0     1001      127     2230 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/matrix_types.rs
+-rw-r--r--   0     1001      127     1401 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/mod.rs
+-rw-r--r--   0     1001      127     3099 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/scalarmath.rs
+-rw-r--r--   0     1001      127     2420 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/sparsevector/mod.rs
+-rw-r--r--   0     1001      127     9757 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/tests/matrix.rs
+-rw-r--r--   0     1001      127       24 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/tests/mod.rs
+-rw-r--r--   0     1001      127     3680 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/tests/vector.rs
+-rw-r--r--   0     1001      127     3976 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/utils.rs
+-rw-r--r--   0     1001      127     5114 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/algebra/vecmath.rs
+-rw-r--r--   0     1001      127       14 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/.gitignore
+-rw-r--r--   0     1001      127      418 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/Project.toml
+-rw-r--r--   0     1001      127     1442 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/src/ClarabelRs.jl
+-rw-r--r--   0     1001      127      218 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/src/MOI_wrapper.jl
+-rw-r--r--   0     1001      127     4930 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/src/interface.jl
+-rw-r--r--   0     1001      127     2570 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/src/types.jl
+-rw-r--r--   0     1001      127     3283 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl
+-rw-r--r--   0     1001      127      955 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/test/test_jump.jl
+-rw-r--r--   0     1001      127     1059 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/ClarabelRs/test/test_problem_depot.jl
+-rw-r--r--   0     1001      127      736 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/README.md
+-rw-r--r--   0     1001      127     4032 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/interface.rs
+-rw-r--r--   0     1001      127       48 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/mod.rs
+-rw-r--r--   0     1001      127     3572 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/julia/types.rs
+-rw-r--r--   0     1001      127     3093 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/lib.rs
+-rw-r--r--   0     1001      127      685 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/.gitignore
+-rw-r--r--   0     1001      127     5633 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/cones_py.rs
+-rw-r--r--   0     1001      127     1000 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/cscmatrix_py.rs
+-rw-r--r--   0     1001      127    15321 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/impl_default_py.rs
+-rw-r--r--   0     1001      127     2588 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/io.rs
+-rw-r--r--   0     1001      127      873 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/mod.rs
+-rw-r--r--   0     1001      127     1765 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/module_py.rs
+-rw-r--r--   0     1001      127      871 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/blas_loader.rs
+-rw-r--r--   0     1001      127     3695 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/blas_types.rs
+-rw-r--r--   0     1001      127     4962 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/blas_wrappers.rs
+-rw-r--r--   0     1001      127      901 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/lapack_loader.rs
+-rw-r--r--   0     1001      127     3803 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/lapack_types.rs
+-rw-r--r--   0     1001      127     6008 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/lapack_wrappers.rs
+-rw-r--r--   0     1001      127     1186 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/python/pyblas/mod.rs
+-rw-r--r--   0     1001      127      117 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/qdldl/mod.rs
+-rw-r--r--   0     1001      127    25421 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/qdldl/qdldl.rs
+-rw-r--r--   0     1001      127     8531 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/qdldl/test.rs
+-rw-r--r--   0     1001      127     9037 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/chordal_info.rs
+-rw-r--r--   0     1001      127    19342 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/augment_compact.rs
+-rw-r--r--   0     1001      127     4977 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/augment_standard.rs
+-rw-r--r--   0     1001      127     2303 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/mod.rs
+-rw-r--r--   0     1001      127     4449 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/psd_completion.rs
+-rw-r--r--   0     1001      127     4311 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/reverse_compact.rs
+-rw-r--r--   0     1001      127     1540 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/decomp/reverse_standard.rs
+-rw-r--r--   0     1001      127    24274 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/merge/clique_graph.rs
+-rw-r--r--   0     1001      127     3028 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/merge/disjoint_set_union.rs
+-rw-r--r--   0     1001      127     2766 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/merge/mod.rs
+-rw-r--r--   0     1001      127      921 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/merge/nomerge.rs
+-rw-r--r--   0     1001      127     4341 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/merge/parent_child.rs
+-rw-r--r--   0     1001      127      460 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/mod.rs
+-rw-r--r--   0     1001      127     1785 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/sparsity_pattern.rs
+-rw-r--r--   0     1001      127    13158 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/chordal/supernode_tree.rs
+-rw-r--r--   0     1001      127    10556 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/compositecone.rs
+-rw-r--r--   0     1001      127    13280 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/expcone.rs
+-rw-r--r--   0     1001      127    13661 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/genpowcone.rs
+-rw-r--r--   0     1001      127     5367 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/mod.rs
+-rw-r--r--   0     1001      127     5738 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/nonnegativecone.rs
+-rw-r--r--   0     1001      127     6478 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/nonsymmetric_common.rs
+-rw-r--r--   0     1001      127    14539 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/powcone.rs
+-rw-r--r--   0     1001      127    13970 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/psdtrianglecone.rs
+-rw-r--r--   0     1001      127    15118 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/socone.rs
+-rw-r--r--   0     1001      127     9188 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/supportedcone.rs
+-rw-r--r--   0     1001      127     3391 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/symmetric_common.rs
+-rw-r--r--   0     1001      127     2852 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/cones/zerocone.rs
+-rw-r--r--   0     1001      127       35 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/mod.rs
+-rw-r--r--   0     1001      127    11788 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
+-rw-r--r--   0     1001      127    12389 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
+-rw-r--r--   0     1001      127     8500 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
+-rw-r--r--   0     1001      127       15 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
+-rw-r--r--   0     1001      127     2764 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
+-rw-r--r--   0     1001      127      757 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/mod.rs
+-rw-r--r--   0     1001      127      517 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/kktsolvers/mod.rs
+-rw-r--r--   0     1001      127      402 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/mod.rs
+-rw-r--r--   0     1001      127      293 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/settings.rs
+-rw-r--r--   0     1001      127    20832 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/solver.rs
+-rw-r--r--   0     1001      127     7651 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/core/traits.rs
+-rw-r--r--   0     1001      127     8443 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/data_updating.rs
+-rw-r--r--   0     1001      127      953 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/equilibration.rs
+-rw-r--r--   0     1001      127    11373 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/info.rs
+-rw-r--r--   0     1001      127    10801 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/info_print.rs
+-rw-r--r--   0     1001      127     8358 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/kktsystem.rs
+-rw-r--r--   0     1001      127      592 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/mod.rs
+-rw-r--r--   0     1001      127     5441 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/presolver.rs
+-rw-r--r--   0     1001      127    11012 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/problemdata.rs
+-rw-r--r--   0     1001      127     2984 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/residuals.rs
+-rw-r--r--   0     1001      127     6231 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/settings.rs
+-rw-r--r--   0     1001      127     2796 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/solution.rs
+-rw-r--r--   0     1001      127     3167 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/solver.rs
+-rw-r--r--   0     1001      127     8670 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/default/variables.rs
+-rw-r--r--   0     1001      127       77 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/implementations/mod.rs
+-rw-r--r--   0     1001      127     1998 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/mod.rs
+-rw-r--r--   0     1001      127      832 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/tests/cones.rs
+-rw-r--r--   0     1001      127       11 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/tests/mod.rs
+-rw-r--r--   0     1001      127      761 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/utils/atomic.rs
+-rw-r--r--   0     1001      127     1327 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/utils/infbounds.rs
+-rw-r--r--   0     1001      127       49 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/solver/utils/mod.rs
+-rw-r--r--   0     1001      127      367 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/stdio/mod.rs
+-rw-r--r--   0     1001      127      109 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/timers/mod.rs
+-rw-r--r--   0     1001      127     5066 2024-05-21 12:09:13.000000 clarabel-0.8.0/src/timers/timers.rs
+-rw-r--r--   0     1001      127     2352 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/api_dimension_checks.rs
+-rw-r--r--   0     1001      127     2328 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_eq_constrained.rs
+-rw-r--r--   0     1001      127     2807 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_expcone.rs
+-rw-r--r--   0     1001      127     1439 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_genpowcone.rs
+-rw-r--r--   0     1001      127     2605 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_lp.rs
+-rw-r--r--   0     1001      127     1382 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_powcone.rs
+-rw-r--r--   0     1001      127     4426 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_qp.rs
+-rw-r--r--   0     1001      127     2493 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_sdp.rs
+-rw-r--r--   0     1001      127     2419 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_socp.rs
+-rw-r--r--   0     1001      127      989 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/basic_unconstrained.rs
+-rw-r--r--   0     1001      127     9191 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/data_updating.rs
+-rw-r--r--   0     1001      127     2600 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/equilibration_bounds.rs
+-rw-r--r--   0     1001      127     1126 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/mixed_conic.rs
+-rw-r--r--   0     1001      127     2408 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/presolve.rs
+-rw-r--r--   0     1001      127     2820 2024-05-21 12:09:13.000000 clarabel-0.8.0/tests/sdp_chordal.rs
+-rw-r--r--   0     1001      127      290 2024-05-21 12:09:13.000000 clarabel-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 clarabel-0.8.0/PKG-INFO
```

### Comparing `clarabel-0.7.1/Cargo.toml` & `clarabel-0.8.0/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "clarabel"
-version = "0.7.1"
+version = "0.8.0"
 authors = ["Paul Goulart <paul.goulart@eng.ox.ac.uk>"]
 edition = "2021"
-rust-version = "1.60"
+rust-version = "1.66"
 license = "Apache-2.0"
 description = "Clarabel Conic Interior Point Solver for Rust / Python"
 readme = "README.md"
 repository = "https://github.com/oxfordcontrol/Clarabel.rs"
 keywords = ["convex", "optimization", "conic", "solver", "linear-programming"]
 categories = ["mathematics"]
 
@@ -27,15 +27,16 @@
 # -------------------------------
 # features
 # -------------------------------
 
 [features]
 
 # enables blas/lapack for SDP support, with blas/lapack src unspecified
-sdp = ["blas","lapack"]
+# also enable packages required for chordal decomposition 
+sdp = ["blas","lapack", "indexmap"]
 
 # explicit configuration options for different blas flavours
 sdp-accelerate = ["sdp", "blas-src/accelerate", "lapack-src/accelerate"]
 sdp-netlib     = ["sdp", "blas-src/netlib", "lapack-src/netlib"]
 sdp-openblas   = ["sdp", "blas-src/openblas", "lapack-src/openblas"]
 sdp-mkl        = ["sdp", "blas-src/intel-mkl", "lapack-src/intel-mkl"]
 sdp-r          = ["sdp", "blas-src/r", "lapack-src/r"]
@@ -47,33 +48,37 @@
 # NB: python builds use scipy shared libraries
 # for blas/lapack, and should *not* explicitly 
 # enable a blas/lapack source package 
 python = ["sdp", "dep:libc", "dep:pyo3", "dep:num-derive"]
 
 
 # -------------------------------
-# blas / lapack configuration
+# SDP configuration
 # -------------------------------
 
 [dependencies.blas]
 version = "0.22.0"
 optional = true
 
 [dependencies.lapack]
 version = "0.19.0"
 optional = true
 
 [dependencies.blas-src]
-version = "0.9"
+version = "0.10"
 optional = true 
 
 [dependencies.lapack-src]
-version = "0.9"
+version = "0.10"
 optional = true 
 
+[dependencies.indexmap]
+version = "2.2"
+optional = true
+
 
 # -------------------------------
 # examples
 # -------------------------------
 
 [[example]]
 name = "lp"
@@ -101,15 +106,14 @@
 
 [[example]]
 name = "sdp"
 path = "examples/rust/example_sdp.rs"
 required-features = ["sdp"]
 
 
-
 # -------------------------------
 # custom build profiles 
 # -------------------------------
 [profile.release-with-debug]
 inherits = "release"
 debug = true
 
@@ -152,9 +156,9 @@
 # ------------------------------
 # enable latex in docs 
 # credit: https://github.com/victe/rust-latex-doc-minimal-example
 # ------------------------------
 
 [package.metadata.docs.rs]
 rustdoc-args = [ "--html-in-header", "./html/rustdocs-header.html" ]
-
+features = ["sdp","sdp-openblas"]
```

### Comparing `clarabel-0.7.1/.github/workflows/ci.yml` & `clarabel-0.8.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 jobs:
   build:
 
     runs-on: macos-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Build
       run: cargo build --verbose --features sdp-accelerate
       
     - name: Run tests
       run: cargo test --verbose --features sdp-accelerate
 
     - name: Install cargo-tarpaulin
       run: cargo install cargo-tarpaulin
 
     - name: Generate code coverage 
       run: |
         cargo tarpaulin --out xml --features sdp-accelerate --exclude-files "src/python/*,src/julia/*"
 
     - name: Upload to codecov.io
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{secrets.CODECOV_TOKEN}}
```

### Comparing `clarabel-0.7.1/.github/workflows/pypi.yaml` & `clarabel-0.8.0/.github/workflows/pypi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
   linux:
     runs-on: ubuntu-latest
     strategy:
        matrix:
         target: [x86_64, i686, aarch64]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
@@ -51,22 +51,21 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
 
   macos:
-    runs-on: macos-latest
+    runs-on: macos-13
     # if: "startsWith(github.ref, 'refs/tags/v')"
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
-          architecture: x64
 
       - name: Install Rust toolchain
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           profile: minimal
           default: true
@@ -97,28 +96,28 @@
           pip install --upgrade pip
           pip install dist/${{ env.PACKAGE_NAME }}-*universal2.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
     # if: "startsWith(github.ref, 'refs/tags/v')"
     strategy:
       matrix:
         target: [x64, x86]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: ${{ matrix.target }}
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
@@ -131,24 +130,24 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
@@ -173,15 +172,15 @@
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - uses: actions/download-artifact@v3
         with:
           name: sdist
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Publish to PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
```

### Comparing `clarabel-0.7.1/.github/workflows/testpypi.yaml` & `clarabel-0.8.0/.github/workflows/testpypi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
   linux:
     runs-on: ubuntu-latest
     strategy:
        matrix:
         target: [x86_64, i686, aarch64]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
@@ -45,16 +45,16 @@
           name: wheels
           path: dist
 
 
   macos:
     runs-on: macos-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: x64
 
       - name: Install Rust toolchain
         uses: actions-rs/toolchain@v1
         with:
@@ -88,27 +88,27 @@
           pip install --upgrade pip
           pip install dist/${{ env.PACKAGE_NAME }}-*universal2.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: ${{ matrix.target }}
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
@@ -121,24 +121,24 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
@@ -162,15 +162,15 @@
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - uses: actions/download-artifact@v3
         with:
           name: sdist
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Publish to Test PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TEST_PYPI_TOKEN }}
         run: |
```

### Comparing `clarabel-0.7.1/CHANGELOG.md` & `clarabel-0.8.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,34 @@
 # Changelog
 
-Changes for the Rust version of Clarabel are documented in this file.   For the Julia version, see [here](https://github.com/oxfordcontrol/Clarabel.jl/blob/main/CHANGELOG.md).
+Changes for the Rust version of Clarabel are documented in this file. For the Julia version, see [here](https://github.com/oxfordcontrol/Clarabel.jl/blob/main/CHANGELOG.md).
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
-Version numbering in this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).  We aim to keep the core solver functionality and minor releases in sync between the Rust/Python and Julia implementations.   Small fixes that affect one implementation only may result in the patch release versions differing.
+Version numbering in this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).  We aim to keep the core solver functionality and minor releases in sync between the Rust/Python and Julia implementations.  Small fixes that affect one implementation only may result in the patch release versions differing.
 
+## [0.8.0] - 2024-21-05
+### Changed 
+
+- implements chordal decomposition for PSD cones [#100](https://github.com/oxfordcontrol/Clarabel.rs/pull/100)
+- updates scaling bounds. Fixes [#96](https://github.com/oxfordcontrol/Clarabel.rs/issues/96)
+
+### Rust specific changes
+
+- Derive debug trait to the solution struct [#97](https://github.com/oxfordcontrol/Clarabel.rs/pull/97). Thanks @nunzioono.
+- Resolve clippy warnings for rustc >=v1.75 [#94](https://github.com/oxfordcontrol/Clarabel.rs/pull/94)
+
+## [0.7.1] - 2024-29-02
+### Changed 
+
+- Fixes a panic / crash condition in PSD scaling step [#78](https://github.com/oxfordcontrol/Clarabel.rs/pull/78)
+
+### Rust specific changes
+
+- Fix to output printing when Python version is run within a Jupyter notebook / Google Colab.  Fixes [#60].
 
 ## [0.7.1] - 2024-29-02
 ### Changed 
 
 - Fixes a panic / crash condition in PSD scaling step [#78](https://github.com/oxfordcontrol/Clarabel.rs/pull/78)
 
 ### Rust specific changes
@@ -116,14 +135,15 @@
 ## [0.2.0] - 2022-07-31
 
 - Rust/python implementation released starting from this version.
 
 - Ported all documentation to the common site [here](https://github.com/oxfordcontrol/ClarabelDocs)
 
 
+[0.8.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.7.1...v0.8.0
 [0.7.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.6.0...v0.7.0
 [0.6.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.4.1...v0.5.0
 [0.4.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.4.0...v0.4.1
 [0.4.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.3.0...v0.4.0
```

### Comparing `clarabel-0.7.1/Cargo.lock` & `clarabel-0.8.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -5,98 +5,104 @@
 [[package]]
 name = "accelerate-src"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "415ed64958754dbe991900f3940677e6a7eefb4d7367afd70d642677b0c7d19d"
 
 [[package]]
-name = "addr2line"
-version = "0.21.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
-dependencies = [
- "gimli",
-]
-
-[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "aho-corasick"
+version = "1.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "amd"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a679e001575697a3bd195813feb57a4718ecc08dc194944015cbc5f6213c2b96"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
-name = "backtrace"
-version = "0.3.69"
+name = "base16ct"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
-dependencies = [
- "addr2line",
- "cc",
- "cfg-if 1.0.0",
- "libc",
- "miniz_oxide",
- "object",
- "rustc-demangle",
-]
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blas"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae980f75c3215bfe8203c349b28149b0f4130a262e072913ccb55f877cd239dc"
 dependencies = [
  "blas-sys",
  "libc",
  "num-complex",
 ]
 
 [[package]]
 name = "blas-src"
-version = "0.9.0"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa443ee19b4cde6cdbd49043eb8964f9dd367b6d98d67f04395958ebfa28f39d"
+checksum = "b95e83dc868db96e69795c0213143095f03de9dd3252f205d4ac716e4076a7e0"
 dependencies = [
  "accelerate-src",
  "intel-mkl-src",
  "netlib-src",
  "openblas-src",
  "r-src",
 ]
@@ -107,45 +113,66 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13b1b279ceb25d7c4faaea95a5f7addbe7d8c34f9462044bd8e630cebcfc2440"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "cc"
-version = "1.0.88"
+name = "block-buffer"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
- "libc",
+ "generic-array",
 ]
 
 [[package]]
-name = "cfg-if"
-version = "0.1.10"
+name = "bumpalo"
+version = "3.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
+
+[[package]]
+name = "cc"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.38"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
+dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
+ "js-sys",
+ "num-traits",
+ "wasm-bindgen",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "clarabel"
-version = "0.7.1"
+version = "0.8.0"
 dependencies = [
  "amd",
  "blas",
  "blas-src",
- "cfg-if 1.0.0",
- "derive_builder",
+ "cfg-if",
+ "derive_builder 0.11.2",
  "enum_dispatch",
- "itertools 0.11.0",
+ "indexmap",
+ "itertools",
  "lapack",
  "lapack-src",
  "lazy_static",
  "libc",
  "num-derive",
  "num-traits",
  "pyo3",
@@ -176,221 +203,281 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
-name = "crc32fast"
-version = "1.4.0"
+name = "cpufeatures"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
- "cfg-if 1.0.0",
+ "libc",
 ]
 
 [[package]]
-name = "curl"
-version = "0.4.46"
+name = "crc32fast"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e2161dd6eba090ff1594084e95fd67aeccf04382ffea77999ea94ed42ec67b6"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
- "curl-sys",
- "libc",
- "openssl-probe",
- "openssl-sys",
- "schannel",
- "socket2",
- "windows-sys",
+ "cfg-if",
 ]
 
 [[package]]
-name = "curl-sys"
-version = "0.4.72+curl-8.6.0"
+name = "crypto-common"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29cbdc8314c447d11e8fd156dcdd031d9e02a7a976163e396b548c03153bc9ea"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
- "cc",
- "libc",
- "libz-sys",
- "openssl-sys",
- "pkg-config",
- "vcpkg",
- "windows-sys",
+ "generic-array",
+ "typenum",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
- "darling_core",
- "darling_macro",
+ "darling_core 0.14.4",
+ "darling_macro 0.14.4",
+]
+
+[[package]]
+name = "darling"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83b2eb4d90d12bdda5ed17de686c2acb4c57914f8f921b8da7e112b5a36f3fe1"
+dependencies = [
+ "darling_core 0.20.9",
+ "darling_macro 0.20.9",
 ]
 
 [[package]]
 name = "darling_core"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
 dependencies = [
  "fnv",
  "ident_case",
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "strsim",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "strsim 0.10.0",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "darling_core"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "strsim 0.11.1",
+ "syn 2.0.65",
+]
+
+[[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
 dependencies = [
- "darling_core",
- "quote 1.0.35",
+ "darling_core 0.14.4",
+ "quote 1.0.36",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "darling_macro"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
+dependencies = [
+ "darling_core 0.20.9",
+ "quote 1.0.36",
+ "syn 2.0.65",
+]
+
+[[package]]
 name = "derive_builder"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d07adf7be193b71cc36b193d0f5fe60b918a3a9db4dad0449f57bcfd519704a3"
 dependencies = [
- "derive_builder_macro",
+ "derive_builder_macro 0.11.2",
+]
+
+[[package]]
+name = "derive_builder"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0350b5cb0331628a5916d6c5c0b72e97393b8b6b03b47a9284f4e7f5a405ffd7"
+dependencies = [
+ "derive_builder_macro 0.20.0",
 ]
 
 [[package]]
 name = "derive_builder_core"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f91d4cfa921f1c05904dc3c57b4a32c38aed3340cce209f3a6fd1478babafc4"
 dependencies = [
- "darling",
- "proc-macro2 1.0.78",
- "quote 1.0.35",
+ "darling 0.14.4",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "derive_builder_core"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
+dependencies = [
+ "darling 0.20.9",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
+]
+
+[[package]]
 name = "derive_builder_macro"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f0314b72bed045f3a68671b3c86328386762c93f82d98c65c3cb5e5f573dd68"
 dependencies = [
- "derive_builder_core",
+ "derive_builder_core 0.11.2",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "dirs"
-version = "2.0.2"
+name = "derive_builder_macro"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
+dependencies = [
+ "derive_builder_core 0.20.0",
+ "syn 2.0.65",
+]
+
+[[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
+name = "directories"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13aea89a5c93364a98e9b37b2fa237effbb694d5cfe01c5b70941f7eb087d5e3"
+checksum = "9a49173b84e034382284f27f1af4dcbbd231ffa358c0fe316541a7337f376a35"
 dependencies = [
- "cfg-if 0.1.10",
- "dirs-sys",
+ "dirs-sys 0.4.1",
 ]
 
 [[package]]
 name = "dirs"
 version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30baa043103c9d0c2a57cf537cc2f35623889dc0d405e6c3cccfadbc81c71309"
 dependencies = [
- "dirs-sys",
+ "dirs-sys 0.3.7",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
-name = "either"
-version = "1.10.0"
+name = "dirs-sys"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
+dependencies = [
+ "libc",
+ "option-ext",
+ "redox_users",
+ "windows-sys 0.48.0",
+]
 
 [[package]]
-name = "enum_dispatch"
-version = "0.3.12"
+name = "either"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
-dependencies = [
- "once_cell",
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 2.0.52",
-]
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
-name = "errno"
-version = "0.3.8"
+name = "enum_dispatch"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
- "libc",
- "windows-sys",
+ "once_cell",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
-name = "failure"
-version = "0.1.8"
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32e9bd16cc02eae7db7ef620b392808b89f6a5e16bb3497d159c6b92a0f4f86"
-dependencies = [
- "backtrace",
- "failure_derive",
-]
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "failure_derive"
-version = "0.1.8"
+name = "errno"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa4da3c766cd7a0db8242e326e9e4e081edd567072893ed320008189715366a4"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 1.0.109",
- "synstructure",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
- "redox_syscall",
- "windows-sys",
+ "redox_syscall 0.4.1",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -419,43 +506,82 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
-name = "gimli"
-version = "0.28.1"
+name = "getset"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "e45727250e75cc04ff2846a66397da8ef2b3db8e40e0cef4df67950a07621eb9"
+dependencies = [
+ "proc-macro-error",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 1.0.109",
+]
 
 [[package]]
-name = "glob"
-version = "0.3.1"
+name = "hashbrown"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows-core",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
@@ -464,84 +590,91 @@
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+dependencies = [
+ "equivalent",
+ "hashbrown",
+]
+
+[[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "intel-mkl-src"
-version = "0.5.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7260b33a735eaebcb942800728b38c5760b125ea5e4346290d78397b5422b894"
+checksum = "2ee70586cd5b3e772a8739a1bd43eaa90d4f4bf0fb2a4edc202e979937ee7f5e"
 dependencies = [
+ "anyhow",
  "intel-mkl-tool",
+ "ocipkg",
 ]
 
 [[package]]
 name = "intel-mkl-tool"
-version = "0.1.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ada23f955fb7d06cb5db9424863caa7251f8f9b525f4c4816144465f77cfded7"
+checksum = "887a16b4537d82227af54d3372971cfa5e0cde53322e60f57584056c16ada1b4"
 dependencies = [
- "curl",
- "dirs 2.0.2",
- "failure",
- "glob",
+ "anyhow",
  "log",
- "pkg-config",
- "tar",
- "zstd",
-]
-
-[[package]]
-name = "itertools"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "284f18f85651fe11e8a991b2adb42cb078325c996ed026d994719efcfca1d54b"
-dependencies = [
- "either",
+ "walkdir",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
+
+[[package]]
+name = "js-sys"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
+dependencies = [
+ "wasm-bindgen",
+]
 
 [[package]]
 name = "lapack"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad676a6b4df7e76a9fd80a0c50c619a3948d6105b62a0ab135f064d99c51d207"
 dependencies = [
  "lapack-sys",
  "libc",
  "num-complex",
 ]
 
 [[package]]
 name = "lapack-src"
-version = "0.9.0"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24c81fcc728418323178fd40407619d0ed26dbbbd1a553693c6290ef5d6698c6"
+checksum = "a960a9d20df9abedf2e136c087c8fcc29f693ed985349bb03fe00816de8b00d2"
 dependencies = [
  "accelerate-src",
  "intel-mkl-src",
  "netlib-src",
  "openblas-src",
  "r-src",
 ]
@@ -559,83 +692,70 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
- "redox_syscall",
-]
-
-[[package]]
-name = "libz-sys"
-version = "1.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "037731f5d3aaa87a5675e895b63ddff1a87624bc29f77004ea829809654e48f6"
-dependencies = [
- "cc",
- "libc",
- "pkg-config",
- "vcpkg",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
@@ -661,17 +781,17 @@
 checksum = "39f41f36bb4d46906d5a72da5b73a804d9de1a7282eb7c89617201acda7b8212"
 dependencies = [
  "cmake",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-derive"
 version = "0.2.5"
@@ -681,28 +801,59 @@
  "proc-macro2 0.4.30",
  "quote 0.6.13",
  "syn 0.15.44",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "object"
-version = "0.32.2"
+name = "oci-spec"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "e423c4f827362c0d8d8da4b1f571270f389ebde73bcd3240a3d23c6d6f61d0f0"
 dependencies = [
- "memchr",
+ "derive_builder 0.20.0",
+ "getset",
+ "serde",
+ "serde_json",
+ "thiserror",
+]
+
+[[package]]
+name = "ocipkg"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9bb3293021f06540803301af45e7ab81693d50e89a7398a3420bdab139e7ba5e"
+dependencies = [
+ "base16ct",
+ "base64",
+ "chrono",
+ "directories",
+ "flate2",
+ "lazy_static",
+ "log",
+ "oci-spec",
+ "regex",
+ "serde",
+ "serde_json",
+ "sha2",
+ "tar",
+ "thiserror",
+ "toml",
+ "ureq",
+ "url",
+ "uuid",
+ "walkdir",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
@@ -724,84 +875,90 @@
 
 [[package]]
 name = "openblas-src"
 version = "0.10.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa4958649f766a1013db4254a852cdf2836764869b6654fa117316905f537363"
 dependencies = [
- "dirs 3.0.2",
+ "dirs",
  "openblas-build",
  "vcpkg",
 ]
 
 [[package]]
 name = "openssl"
 version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags 2.4.2",
- "cfg-if 1.0.0",
+ "bitflags 2.5.0",
+ "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 2.0.52",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.101"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -815,38 +972,62 @@
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 1.0.109",
+ "version_check",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "version_check",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "0.4.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf3d2011ab5c909338f7887f4fc896d35932e29146c12c8d01da6b22a80ba759"
 dependencies = [
- "unicode-xid 0.1.0",
+ "unicode-xid",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
@@ -876,49 +1057,49 @@
 
 [[package]]
 name = "pyo3-macros"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
- "proc-macro2 1.0.78",
+ "proc-macro2 1.0.83",
  "pyo3-macros-backend",
- "quote 1.0.35",
- "syn 2.0.52",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
- "proc-macro2 1.0.78",
+ "proc-macro2 1.0.83",
  "pyo3-build-config",
- "quote 1.0.35",
- "syn 2.0.52",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "quote"
 version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ce23b6b870e8f94f81fb0a363d65d86675884b34a09043c81e5562f11c1f8e1"
 dependencies = [
  "proc-macro2 0.4.30",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
- "proc-macro2 1.0.78",
+ "proc-macro2 1.0.83",
 ]
 
 [[package]]
 name = "r-src"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea397956e1043a8d947ea84b13971d9cb30fce65ca66a921081755ff2e899b6a"
@@ -929,41 +1110,102 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
-name = "rustc-demangle"
-version = "0.1.23"
+name = "regex"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+
+[[package]]
+name = "ring"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "getrandom",
+ "libc",
+ "spin",
+ "untrusted",
+ "windows-sys 0.52.0",
+]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "rustls"
+version = "0.22.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-pki-types",
+ "rustls-webpki",
+ "subtle",
+ "zeroize",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f1fb85efa936c42c6d5fc28d2629bb51e4b2f4b8a5211e297d599cc5a093792"
@@ -973,33 +1215,44 @@
  "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "2.1.1"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f48172685e6ff52a556baa527774f61fcaa884f59daf3375c62a3f1cd2549dab"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
  "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.3.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
+
+[[package]]
+name = "rustls-webpki"
+version = "0.102.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
+dependencies = [
+ "ring",
+ "rustls-pki-types",
+ "untrusted",
+]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1008,145 +1261,161 @@
 
 [[package]]
 name = "schannel"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 2.0.52",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "smallvec"
-version = "1.13.1"
+name = "serde_spanned"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "79e674e01f999af37c49f70a6ede167a8a60b2503e56c5599532a65baa5969a0"
+dependencies = [
+ "serde",
+]
 
 [[package]]
-name = "socket2"
-version = "0.5.6"
+name = "sha2"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
- "libc",
- "windows-sys",
+ "cfg-if",
+ "cpufeatures",
+ "digest",
 ]
 
 [[package]]
+name = "smallvec"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
+name = "spin"
+version = "0.9.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
+
+[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
+name = "strsim"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
+
+[[package]]
+name = "subtle"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
+
+[[package]]
 name = "syn"
 version = "0.15.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ca4b3b69a77cbe1ffc9e198781b7acb0c7365a883670e8f1c1bc66fba79a5c5"
 dependencies = [
  "proc-macro2 0.4.30",
  "quote 0.6.13",
- "unicode-xid 0.1.0",
+ "unicode-xid",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
  "unicode-ident",
 ]
 
 [[package]]
-name = "synstructure"
-version = "0.12.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
-dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 1.0.109",
- "unicode-xid 0.2.4",
-]
-
-[[package]]
 name = "tar"
 version = "0.4.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b16afcea1f22891c49a00c751c7b63b2233284064f11a200fc624137c51e2ddb"
 dependencies = [
  "filetime",
  "libc",
@@ -1161,38 +1430,38 @@
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "fastrand",
  "rustix",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
- "proc-macro2 1.0.78",
- "quote 1.0.35",
- "syn 2.0.52",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1203,14 +1472,54 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
+name = "toml"
+version = "0.8.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a4e43f8cc456c9704c851ae29c67e17ef65d2c30017c17a9765b89c382dc8bba"
+dependencies = [
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "toml_edit",
+]
+
+[[package]]
+name = "toml_datetime"
+version = "0.6.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "toml_edit"
+version = "0.22.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c127785850e8c20836d49732ae6abfa47616e60bf9d9f57c43c250361a9db96c"
+dependencies = [
+ "indexmap",
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
+name = "typenum"
+version = "1.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
@@ -1230,58 +1539,79 @@
 [[package]]
 name = "unicode-xid"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc72304796d0818e357ead4e000d19c9c174ab23dc11093ac919054d20a6a7fc"
 
 [[package]]
-name = "unicode-xid"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
-
-[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "untrusted"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
+
+[[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
  "base64",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
+ "rustls",
  "rustls-native-certs",
+ "rustls-pki-types",
+ "rustls-webpki",
+ "serde",
+ "serde_json",
  "url",
+ "webpki-roots",
 ]
 
 [[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "walkdir"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
@@ -1290,14 +1620,77 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
+dependencies = [
+ "quote 1.0.36",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
+dependencies = [
+ "proc-macro2 1.0.83",
+ "quote 1.0.36",
+ "syn 2.0.65",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
+
+[[package]]
+name = "webpki-roots"
+version = "0.26.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
+dependencies = [
+ "rustls-pki-types",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -1307,34 +1700,52 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.5",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1346,145 +1757,136 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
-name = "xattr"
-version = "1.3.1"
+name = "winnow"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
- "libc",
- "linux-raw-sys",
- "rustix",
-]
-
-[[package]]
-name = "zstd"
-version = "0.5.4+zstd.1.4.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69996ebdb1ba8b1517f61387a883857818a66c8a295f487b1ffd8fd9d2c82910"
-dependencies = [
- "zstd-safe",
+ "memchr",
 ]
 
 [[package]]
-name = "zstd-safe"
-version = "2.0.6+zstd.1.4.7"
+name = "xattr"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98aa931fb69ecee256d44589d19754e61851ae4769bf963b385119b1cc37a49e"
+checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
  "libc",
- "zstd-sys",
+ "linux-raw-sys",
+ "rustix",
 ]
 
 [[package]]
-name = "zstd-sys"
-version = "1.4.18+zstd.1.4.7"
+name = "zeroize"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1e6e8778706838f43f771d80d37787cb2fe06dafe89dd3aebaf6721b9eaec81"
-dependencies = [
- "cc",
- "glob",
- "itertools 0.9.0",
- "libc",
-]
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `clarabel-0.7.1/LICENSE.md` & `clarabel-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/README.md` & `clarabel-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 </picture>
 <h1 align="center" margin=0px>
 Interior Point Conic Optimization for Rust and Python
 </h1>
 <p align="center">
    <a href="https://github.com/oxfordcontrol/Clarabel.rs/actions"><img src="https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/oxfordcontrol/Clarabel.rs"><img src="https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/main/graph/badge.svg"></a>
-  <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
+  <a href="https://clarabel.org"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.7.1-blue.svg"></a>
+  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.8.0-blue.svg"></a>
 </p>
 
 <p align="center">
   <a href="#features">Features</a> •
   <a href="#installation">Installation</a> •
   <a href="#license-">License</a> •
-  <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable">Documentation</a>
+  <a href="https://clarabel.org">Documentation</a>
 </p>
 
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver for convex optimization problems using a novel homogeneous embedding.  Clarabel.rs solves the following problem:
 
 $$
 \begin{array}{r}
 \text{minimize} & \frac{1}{2}x^T P x + q^T x\\\\[2ex]
@@ -38,15 +38,15 @@
 and data matrices
 $P=P^\top \succeq 0$,
 $q \in \mathbb{R}^n$,
 $A \in \mathbb{R}^{m \times n}$, and
 $b \in \mathbb{R}^m$.
 The convex set $\mathcal{K}$ is a composition of convex cones.
 
-__For more information see the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/ClarabelDocs/stable) |  [dev](https://oxfordcontrol.github.io/ClarabelDocs/dev)).__
+__For more information see the Clarabel Documentation ([stable](https://clarabel.org) |  [dev](https://clarabel.org/dev)).__
 
 Clarabel is also available in a Julia implementation.  See [here](https://github.com/oxfordcontrol/Clarabel.jl).
  
 
 ## Features
 
 * __Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves problems with exponential, power cone and generalized power cone constraints.
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
                               [Clarabel.jl logo]
       ************ IInntteerriioorr PPooiinntt CCoonniicc OOppttiimmiizzaattiioonn ffoorr RRuusstt aanndd PPyytthhoonn ************
           _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_w_o_r_k_f_l_o_w_s_/_c_i_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_b_r_a_n_c_h_/
    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_s_t_a_b_l_e_-
 _p_u_r_p_l_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/
-                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._7_._1_-_b_l_u_e_._s_v_g_]
+                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._8_._0_-_b_l_u_e_._s_v_g_]
             _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _L_i_c_e_n_s_e â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver
 for convex optimization problems using a novel homogeneous embedding.
 Clarabel.rs solves the following problem: $$ \begin{array}{r} \text{minimize} &
 \frac{1}{2}x^T P x + q^T x\\\\[2ex] \text{subject to} & Ax + s = b \\\\[1ex] &
 s \in \mathcal{K} \end{array} $$ with decision variables $x \in \mathbb{R}^n$,
 $s \in \mathbb{R}^m$ and data matrices $P=P^\top \succeq 0$, $q \in \mathbb
 {R}^n$, $A \in \mathbb{R}^{m \times n}$, and $b \in \mathbb{R}^m$. The convex
 set $\mathcal{K}$ is a composition of convex cones. __For more information see
-the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/
-ClarabelDocs/stable) | [dev](https://oxfordcontrol.github.io/ClarabelDocs/
-dev)).__ Clarabel is also available in a Julia implementation. See [here]
-(https://github.com/oxfordcontrol/Clarabel.jl). ## Features * __Versatile__:
-Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-
-order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves
-problems with exponential, power cone and generalized power cone constraints. *
-__Quadratic objectives__: Unlike interior point solvers based on the standard
-homogeneous self-dual embedding (HSDE), Clarabel.rs handles quadratic
-objectives without requiring any epigraphical reformulation of the objective.
-It can therefore be significantly faster than other HSDE-based solvers for
-problems with quadratic objective functions. * __Infeasibility detection__:
-Infeasible problems are detected using a homogeneous embedding technique. *
-__Open Source__: Our code is available on [GitHub](https://github.com/
-oxfordcontrol/Clarabel.rs) and distributed under the Apache 2.0 License #
-Installation Clarabel can be imported to Cargo based Rust projects by adding
-```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml` file.
-To install from source, see the [Rust Installation Documentation](https://
-oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
+the Clarabel Documentation ([stable](https://clarabel.org) | [dev](https://
+clarabel.org/dev)).__ Clarabel is also available in a Julia implementation. See
+[here](https://github.com/oxfordcontrol/Clarabel.jl). ## Features *
+__Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs
+(QPs), second-order cone programs (SOCPs) and semidefinite programs (SDPs). It
+also solves problems with exponential, power cone and generalized power cone
+constraints. * __Quadratic objectives__: Unlike interior point solvers based on
+the standard homogeneous self-dual embedding (HSDE), Clarabel.rs handles
+quadratic objectives without requiring any epigraphical reformulation of the
+objective. It can therefore be significantly faster than other HSDE-based
+solvers for problems with quadratic objective functions. * __Infeasibility
+detection__: Infeasible problems are detected using a homogeneous embedding
+technique. * __Open Source__: Our code is available on [GitHub](https://
+github.com/oxfordcontrol/Clarabel.rs) and distributed under the Apache 2.0
+License # Installation Clarabel can be imported to Cargo based Rust projects by
+adding ```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml`
+file. To install from source, see the [Rust Installation Documentation](https:/
+/oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
 Python interface to the solver: ``` pip install clarabel ``` To install the
 Python interface from source, see the [Python Installation Documentation]
 (https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
 ## License ð This project is licensed under the Apache License 2.0 - see the
 [LICENSE.md](LICENSE.md) file for details.
```

### Comparing `clarabel-0.7.1/examples/python/example_expcone.py` & `clarabel-0.8.0/examples/python/example_expcone.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/python/example_powcone.py` & `clarabel-0.8.0/examples/python/example_powcone.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/python/example_qp.py` & `clarabel-0.8.0/examples/python/example_qp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/python/example_sdp.py` & `clarabel-0.8.0/examples/python/example_sdp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/python/example_socp.py` & `clarabel-0.8.0/examples/python/example_socp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_box.rs` & `clarabel-0.8.0/examples/rust/example_box.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_expcone.rs` & `clarabel-0.8.0/examples/rust/example_expcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_lp.rs` & `clarabel-0.8.0/examples/rust/example_lp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_powcone.rs` & `clarabel-0.8.0/examples/rust/example_powcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_qp.rs` & `clarabel-0.8.0/examples/rust/example_qp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_sdp.rs` & `clarabel-0.8.0/examples/rust/example_sdp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/examples/rust/example_socp.rs` & `clarabel-0.8.0/examples/rust/example_socp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/html/rustdocs-header.html` & `clarabel-0.8.0/html/rustdocs-header.html`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/algebra/csc/core.rs` & `clarabel-0.8.0/src/algebra/csc/core.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{Adjoint, FloatT, MatrixShape, ShapedMatrix, SparseFormatError, Symmetric};
-use std::iter::zip;
+use crate::algebra::permute;
+use crate::algebra::utils::sortperm_by;
+use crate::algebra::{Adjoint, MatrixShape, ShapedMatrix, SparseFormatError, Symmetric};
+use num_traits::Num;
+use std::iter::{repeat, zip};
 
 /// Sparse matrix in standard Compressed Sparse Column (CSC) format
 ///
 /// __Example usage__ : To construct the 3 x 3 matrix
 /// ```text
 /// A = [1.  3.  5.]
 ///     [2.  0.  6.]
@@ -63,28 +66,28 @@
 ///        [3.0, 0.0],
 ///        [0.0, 4.0]]);
 ///
 impl<'a, I, J, T> From<I> for CscMatrix<T>
 where
     I: IntoIterator<Item = J>,
     J: IntoIterator<Item = &'a T>,
-    T: FloatT,
+    T: Num + Copy + 'a,
 {
     #[allow(clippy::needless_range_loop)]
     fn from(rows: I) -> CscMatrix<T> {
         let rows: Vec<Vec<T>> = rows
             .into_iter()
             .map(|r| r.into_iter().copied().collect())
             .collect();
 
         let m = rows.len();
         let n = rows.iter().map(|r| r.len()).next().unwrap_or(0);
 
         assert!(rows.iter().all(|r| r.len() == n));
-        let nnz = rows.iter().flatten().filter(|&&v| v != T::zero()).count();
+        let nnz = rows.iter().flatten().filter(|&v| *v != T::zero()).count();
 
         let mut colptr = Vec::with_capacity(n + 1);
         let mut rowval = Vec::with_capacity(nnz);
         let mut nzval = Vec::<T>::with_capacity(nnz);
 
         colptr.push(0);
         for c in 0..n {
@@ -106,15 +109,15 @@
             nzval,
         }
     }
 }
 
 impl<T> CscMatrix<T>
 where
-    T: FloatT,
+    T: Num + Copy,
 {
     /// `CscMatrix` constructor.
     ///
     /// # Panics
     /// Makes rudimentary dimensional compatibility checks and panics on
     /// failure.   This constructor does __not__
     /// ensure that rows indices are all in bounds or that data is arranged
@@ -132,14 +135,80 @@
             n,
             colptr,
             rowval,
             nzval,
         }
     }
 
+    /// `CscMatrix` constructor from data in triplet format.
+    ///
+    /// # Panics
+    /// Makes rudimentary dimensional compatibility checks and panics on
+    /// failure.   Data can be provided unsorted.   Repeated values are added.
+    ///
+
+    pub fn new_from_triplets(m: usize, n: usize, I: Vec<usize>, J: Vec<usize>, V: Vec<T>) -> Self {
+        assert_eq!(I.len(), J.len());
+        assert_eq!(I.len(), V.len());
+
+        let mut M = CscMatrix::spalloc((m, n), V.len());
+
+        let mut p = vec![0; V.len()];
+
+        // use M.rowptr as temporary workspace
+        M.rowval.iter_mut().enumerate().for_each(|(i, p)| *p = i);
+
+        // sort by column, then by row
+        sortperm_by(&mut p, &M.rowval, |&a, &b| {
+            J[a].cmp(&J[b]).then(I[a].cmp(&I[b]))
+        });
+
+        // map data into the matrix in sorted order
+        permute(&mut M.rowval, &I, &p);
+        permute(&mut M.nzval, &V, &p);
+
+        // assemble the column counts
+        for &c in J.iter() {
+            M.colptr[c] += 1;
+        }
+
+        // make a second pass to consolidate repeated entries
+        // within each column
+        let mut readidx = 0;
+        let mut writeidx = 0;
+
+        for col in 0..n {
+            let nentries = M.colptr[col]; //entries in this column
+            for j in 0..nentries {
+                // non-repeated or first entry in column
+                if j == 0 || M.rowval[readidx] != M.rowval[readidx - 1] {
+                    if writeidx != readidx {
+                        M.rowval[writeidx] = M.rowval[readidx];
+                        M.nzval[writeidx] = M.nzval[readidx];
+                    }
+                    writeidx += 1;
+                    readidx += 1;
+                }
+                // repeated row entry with value to be consolidated
+                else {
+                    M.nzval[writeidx - 1] = M.nzval[writeidx - 1] + M.nzval[readidx];
+                    M.colptr[col] -= 1;
+                    readidx += 1;
+                }
+            }
+        }
+
+        M.rowval.resize(writeidx, 0);
+        M.nzval.resize(writeidx, T::zero());
+
+        M.colcount_to_colptr();
+
+        M
+    }
+
     /// allocate space for a sparse matrix with `nnz` elements
 
     pub fn spalloc(size: (usize, usize), nnz: usize) -> Self {
         let (m, n) = size;
         let mut colptr = vec![0; n + 1];
         let rowval = vec![0; nnz];
         let nzval = vec![T::zero(); nnz];
@@ -158,14 +227,65 @@
         let colptr = (0usize..=n).collect();
         let rowval = (0usize..n).collect();
         let nzval = vec![T::one(); n];
 
         CscMatrix::new(n, n, colptr, rowval, nzval)
     }
 
+    /// squeeze out entries that are == T::zero()
+    pub fn dropzeros(&mut self) {
+        // this function could possibly be generalized to allow filtering
+        // on a more general test, similar to fkeep! in Julia sparse matrix
+        // internals.  Then could be used as a filter for triu matrix etc
+
+        // Sweep through columns, rewriting kept elements in their new positions
+        // and updating the column pointers accordingly as we go.
+        let mut writeidx: usize = 0;
+        let mut first: usize = 0;
+
+        for col in 0..self.ncols() {
+            let last = self.colptr[col + 1];
+
+            for readidx in first..last {
+                let val = self.nzval[readidx];
+                let row = self.rowval[readidx];
+
+                // If nonzero and a shift so far, move the value
+                if val != T::zero() {
+                    if writeidx != readidx {
+                        self.nzval[writeidx] = val;
+                        self.rowval[writeidx] = row;
+                    }
+                    writeidx += 1;
+                }
+            }
+
+            first = self.colptr[col + 1];
+            self.colptr[col + 1] = writeidx;
+        }
+
+        self.rowval.resize(writeidx, 0);
+        self.nzval.resize(writeidx, T::zero());
+    }
+
+    /// Return matrix data in triplet format.
+    ///
+    #[cfg_attr(not(sdp), allow(dead_code))]
+    pub(crate) fn findnz(&self) -> (Vec<usize>, Vec<usize>, Vec<T>) {
+        let I = self.rowval.clone();
+        let mut J = Vec::with_capacity(self.nnz());
+        let V = self.nzval.clone();
+
+        for c in 0..self.ncols() {
+            let times = self.colptr[c + 1] - self.colptr[c];
+            J.extend(repeat(c).take(times));
+        }
+        (I, J, V)
+    }
+
     /// number of nonzeros
     pub fn nnz(&self) -> usize {
         self.colptr[self.n]
     }
 
     /// transpose
     pub fn t(&self) -> Adjoint<'_, Self> {
@@ -353,14 +473,50 @@
         let rows_in_this_column = &self.rowval[first..last];
         match rows_in_this_column.binary_search(&row) {
             Ok(idx) => Some(self.nzval[first + idx]),
             Err(_) => None,
         }
     }
 
+    /// Sets a value at a given (row,col) index, allocating
+    /// additional space in the matrix if required.  
+    ///
+    /// # Panics
+    /// Panics if the given index is out of bounds.
+    pub fn set_entry(&mut self, idx: (usize, usize), value: T) {
+        let (row, col) = idx;
+        assert!(row < self.nrows() && col < self.ncols());
+
+        let first = self.colptr[col];
+        let last = self.colptr[col + 1];
+        let rows_in_this_column = &self.rowval[first..last];
+
+        let i = rows_in_this_column.partition_point(|&x| x < row);
+
+        if i == rows_in_this_column.len() || rows_in_this_column[i] != row {
+            // don't allocate space for insertion of new zeros
+            if value == T::zero() {
+                return;
+            }
+
+            // the element must be inserted, then col counts rebuilt
+            self.rowval.insert(first + i, row);
+            self.nzval.insert(first + i, value);
+
+            // a bit wasteful since we only really need to
+            // rebuil from the insertion point onwards
+            self.colptr_to_colcount();
+            self.colptr[col] += 1;
+            self.colcount_to_colptr();
+        } else {
+            // the element already exists, so overwrite it
+            self.nzval[first + i] = value;
+        }
+    }
+
     /// Returns the (row,col) coordinates of the given linear index.
     ///
     /// # Panics
     /// Panics if the given index is out of bounds.
     pub fn index_to_coord(&self, idx: usize) -> (usize, usize) {
         assert!(idx < self.nnz());
         let row = self.rowval[idx];
@@ -410,15 +566,15 @@
 /// let B : CscMatrix = At.into(); //Concrete form.  Allocates and copies.
 ///
 /// assert_eq!(A, B);
 ///
 /// ```
 impl<'a, T> From<Adjoint<'a, CscMatrix<T>>> for CscMatrix<T>
 where
-    T: FloatT,
+    T: Num + Copy,
 {
     fn from(M: Adjoint<'a, CscMatrix<T>>) -> CscMatrix<T> {
         let src = M.src;
 
         let (m, n) = (src.n, src.m);
         let mut A = CscMatrix::spalloc((m, n), src.nnz());
 
@@ -487,14 +643,43 @@
     assert_eq!(A.get_entry((1, 3)), None);
     assert_eq!(A.get_entry((2, 3)), None);
     assert_eq!(A.get_entry((4, 3)), None);
     assert_eq!(A.get_entry((3, 4)), None);
 }
 
 #[test]
+fn test_csc_set_entry() {
+    let mut A = CscMatrix::from(&[
+        [0.0, 3.0, 6.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 4.0, 7.0, 8.0],
+        [2.0, 5.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0],
+    ]);
+
+    let B = CscMatrix::from(&[
+        [0.0, 3.0, -6.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 4.0, 7.0, -8.0],
+        [2.0, 5.0, 10.0, 0.0],
+        [0.0, 0.0, 0.0, 11.0],
+    ]);
+
+    // overwrite existing entries
+    A.set_entry((0, 2), -6.0);
+    A.set_entry((2, 3), -8.0);
+
+    // add new entries
+    A.set_entry((3, 2), 10.0);
+    A.set_entry((4, 3), 11.0);
+
+    assert_eq!(A, B);
+}
+
+#[test]
 fn test_csc_index_to_coord() {
     let A = CscMatrix::from(&[
         [0.0, 4.0, 0.0, 0.0, 12.0],
         [1.0, 5.0, 0.0, 0.0, 0.0],
         [0.0, 6.0, 0.0, 0.0, 13.0],
         [2.0, 7.0, 10.0, 0.0, 0.0],
         [0.0, 8.0, 11.0, 0.0, 14.0],
@@ -533,7 +718,87 @@
     ])
         .into();
 
     let B: CscMatrix = A.t().into(); //Concrete form.  Allocates and copies.
 
     assert_eq!(B, T);
 }
+
+#[test]
+fn test_triplets() {
+    let A: CscMatrix = (&[
+        [1., 0., 0., 5.], //
+        [0., 0., 3., 0.], //
+        [2., 0., 4., 0.],
+    ])
+        .into();
+
+    let cols = vec![0, 0, 2, 2, 3];
+    let rows = vec![0, 2, 1, 2, 0];
+    let vals = vec![1., 2., 3., 4., 5.];
+
+    // extract triplet format data and compare
+    let (I, J, V) = A.findnz();
+    assert_eq!(I, rows);
+    assert_eq!(J, cols);
+    assert_eq!(V, vals);
+
+    // construct from triplets and compare
+    let B: CscMatrix = CscMatrix::new_from_triplets(3, 4, rows, cols, vals);
+    assert_eq!(A, B);
+
+    // same thing, but with data in the wrong order
+    let cols = vec![2, 0, 2, 0, 3];
+    let rows = vec![2, 2, 1, 0, 0];
+    let vals = vec![4., 2., 3., 1., 5.];
+
+    let B: CscMatrix = CscMatrix::new_from_triplets(3, 4, rows, cols, vals);
+
+    assert_eq!(A, B);
+
+    // case with repeated entries, unsorted
+
+    let A: CscMatrix<isize> = (&[
+        [0, 0, 0],   //
+        [-20, 0, 0], //
+        [-20, -20, 0],
+    ])
+        .into();
+
+    let rows = vec![1, 2, 2, 1, 2, 2];
+    let cols = vec![0, 0, 1, 0, 0, 1];
+    let vals = vec![-10, -10, -10, -10, -10, -10];
+
+    let B = CscMatrix::new_from_triplets(3, 3, rows, cols, vals);
+    assert_eq!(A, B);
+}
+
+#[test]
+fn test_drop_zeros() {
+    let mut A = CscMatrix::from(&[
+        [0.0, 3.0, 6.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 4.0, 7.0, 8.0],
+        [2.0, 5.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0],
+    ]);
+
+    // same, but with 2,6,7,8 set to zero
+    let B = CscMatrix::from(&[
+        [0.0, 3.0, 0.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 4.0, 0.0, 0.0],
+        [0.0, 5.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0],
+    ]);
+
+    // overwrite existing entries
+    let dropped = [2, 6, 7, 8];
+    for idx in dropped {
+        A.nzval[idx - 1] = 0.0;
+    }
+
+    //squeeze out the zeros
+    A.dropzeros();
+
+    assert_eq!(A, B);
+}
```

### Comparing `clarabel-0.7.1/src/algebra/csc/matrix_math.rs` & `clarabel-0.8.0/src/algebra/csc/matrix_math.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 use crate::algebra::*;
 use std::iter::zip;
 
-impl<T: FloatT> MatrixVectorMultiply for CscMatrix<T> {
-    type T = T;
-
+impl<T: FloatT> MatrixVectorMultiply<T> for CscMatrix<T> {
     fn gemv(&self, y: &mut [T], x: &[T], a: T, b: T) {
         _csc_axpby_N(self, y, x, a, b);
     }
 }
 
-impl<T: FloatT> MatrixVectorMultiply for Adjoint<'_, CscMatrix<T>> {
-    type T = T;
-
+impl<T: FloatT> MatrixVectorMultiply<T> for Adjoint<'_, CscMatrix<T>> {
     fn gemv(&self, y: &mut [T], x: &[T], a: T, b: T) {
         _csc_axpby_T(self.src, y, x, a, b);
     }
 }
 
-impl<T: FloatT> SymMatrixVectorMultiply for Symmetric<'_, CscMatrix<T>> {
-    type T = T;
-
+impl<T: FloatT> SymMatrixVectorMultiply<T> for Symmetric<'_, CscMatrix<T>> {
     fn symv(&self, y: &mut [T], x: &[T], a: T, b: T) {
         _csc_symv_unsafe(self.src, y, x, a, b);
     }
 }
 
-impl<T: FloatT> MatrixMath for CscMatrix<T> {
-    type T = T;
-
-    //scalar mut operations
-    fn scale(&mut self, c: T) {
-        self.nzval.scale(c);
+impl<T: FloatT> MatrixMath<T> for CscMatrix<T> {
+    fn col_sums(&self, sums: &mut [T]) {
+        assert_eq!(self.n, sums.len());
+        for (col, sum) in sums.iter_mut().enumerate() {
+            let rng = self.colptr[col]..self.colptr[col + 1];
+            *sum = self.nzval[rng].sum();
+        }
     }
 
-    fn negate(&mut self) {
-        self.nzval.negate();
+    fn row_sums(&self, sums: &mut [T]) {
+        assert_eq!(self.m, sums.len());
+        sums.fill(T::zero());
+        for (&row, &val) in zip(&self.rowval, &self.nzval) {
+            sums[row] += val;
+        }
     }
 
     fn col_norms(&self, norms: &mut [T]) {
         norms.fill(T::zero());
         self.col_norms_no_reset(norms);
     }
 
@@ -82,14 +81,29 @@
         assert_eq!(self.rowval.len(), *self.colptr.last().unwrap());
 
         for (row, val) in zip(&self.rowval, &self.nzval) {
             norms[*row] = T::max(norms[*row], T::abs(*val));
         }
     }
 
+    fn quad_form(&self, y: &[T], x: &[T]) -> T {
+        _csc_quad_form(self, y, x)
+    }
+}
+
+impl<T: FloatT> MatrixMathMut<T> for CscMatrix<T> {
+    //scalar mut operations
+    fn scale(&mut self, c: T) {
+        self.nzval.scale(c);
+    }
+
+    fn negate(&mut self) {
+        self.nzval.negate();
+    }
+
     fn lscale(&mut self, l: &[T]) {
         for (val, row) in zip(&mut self.nzval, &self.rowval) {
             *val *= l[*row];
         }
     }
 
     fn rscale(&mut self, r: &[T]) {
@@ -111,18 +125,14 @@
             let rows = &self.rowval[first..last];
 
             for (val, row) in zip(vals, rows) {
                 *val *= l[*row] * ri;
             }
         }
     }
-
-    fn quad_form(&self, y: &[T], x: &[T]) -> T {
-        _csc_quad_form(self, y, x)
-    }
 }
 
 #[allow(non_snake_case)]
 fn _csc_symv_safe<T: FloatT>(A: &CscMatrix<T>, y: &mut [T], x: &[T], a: T, b: T) {
     y.scale(b);
 
     assert!(x.len() == A.n);
@@ -147,34 +157,31 @@
 }
 
 // Safety: The function below checks that x and y are compatible with
 // the dimensions of A, so safety is assured so long as the the matrix
 // A as rowval and colptr arrays that are consistent with its dimension.
 // A bounds checked version is provided above.
 //
-// This `unsafe`d version is preferred the multiplication K*x, with K
-// the symmetric KKT matrix, is used heavily in iterative refinement of
+// This `unsafe`d version is preferred to the multiplication K*x, with K
+// the symmetric KKT matrix, and is used heavily in iterative refinement of
 // direct linear solves.
 #[allow(non_snake_case)]
 fn _csc_symv_unsafe<T: FloatT>(A: &CscMatrix<T>, y: &mut [T], x: &[T], a: T, b: T) {
     y.scale(b);
 
     assert!(x.len() == A.n);
     assert!(y.len() == A.n);
     assert!(A.n == A.m);
     unsafe {
         for (col, &xcol) in x.iter().enumerate() {
             let first = *A.colptr.get_unchecked(col);
             let last = *A.colptr.get_unchecked(col + 1);
 
-            for j in first..last {
-                let row = *A.rowval.get_unchecked(j);
-                let Aij = *A.nzval.get_unchecked(j);
+            for (&row, &Aij) in zip(&A.rowval[first..last], &A.nzval[first..last]) {
                 *y.get_unchecked_mut(row) += a * Aij * xcol;
-
                 if row != col {
                     //don't double up on the diagonal
                     *y.get_unchecked_mut(col) += a * Aij * (*x.get_unchecked(row));
                 }
             }
         }
     }
```

### Comparing `clarabel-0.7.1/src/algebra/csc/utils.rs` & `clarabel-0.8.0/src/algebra/csc/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 //---------------------------------------------------------
 // low-level internal utilities for counting / filling entries
 // in block partitioned sparse matrices.
 //---------------------------------------------------------
 
-use crate::algebra::{CscMatrix, FloatT, MatrixShape, MatrixTriangle};
+use crate::algebra::{CscMatrix, MatrixShape, MatrixTriangle};
+use num_traits::Num;
 use std::iter::zip;
 
 impl<T> CscMatrix<T>
 where
-    T: FloatT,
+    T: Num + Copy,
 {
     // increment self.colptr by the number of nonzeros
     // in a dense upper/lower triangle on the diagonal.
     pub(crate) fn colcount_dense_triangle(
         &mut self,
         initcol: usize,
         blockcols: usize,
@@ -243,23 +244,34 @@
                 self.rowval[dest] = i + initcol;
                 self.nzval[dest] = T::zero(); //structural zero
                 self.colptr[i] += 1;
             }
         }
     }
 
+    // treats self.colptr as a vector of counts for entries in each column,
+    // and rebuilds a valid colptr from it
     pub(crate) fn colcount_to_colptr(&mut self) {
         let mut currentptr = 0;
         for p in &mut self.colptr {
             let count = *p;
             *p = currentptr;
             currentptr += count;
         }
     }
 
+    // converts the colptr vector a vector of entry counts for each column
+    // the final entry is set to zero
+    pub(crate) fn colptr_to_colcount(&mut self) {
+        for i in 0..self.n {
+            self.colptr[i] = self.colptr[i + 1] - self.colptr[i];
+        }
+        self.colptr[self.n] = 0;
+    }
+
     pub(crate) fn backshift_colptrs(&mut self) {
         self.colptr.rotate_right(1);
         self.colptr[0] = 0;
     }
 
     pub(crate) fn count_diagonal_entries(&self) -> usize {
         let mut count = 0;
```

### Comparing `clarabel-0.7.1/src/algebra/dense/blas.rs` & `clarabel-0.8.0/src/algebra/dense/blas/traits.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,27 @@
         extern crate blas_src;
         extern crate lapack_src;
         use lapack::*;
         use blas::*;
     }
 }
 
-
-
-
 pub trait BlasFloatT: 
     private::BlasFloatSealed 
     + XsyevrScalar 
     + XpotrfScalar 
+    + XpotrsScalar 
     + XgesddScalar 
     + XgesvdScalar 
     + XgemmScalar 
     + XgemvScalar 
     + XsymvScalar 
     + XsyrkScalar
     + Xsyr2kScalar
+    + XgesvScalar
 {}
 
 cfg_if::cfg_if! {
   if #[cfg(not(feature="sdp-r"))] {
 	// R blas/lapack only provides double precision routines
 	impl BlasFloatT for f32 {}
   }
@@ -96,37 +95,54 @@
 
 pub trait XpotrfScalar: Sized {
     fn xpotrf(
         uplo: u8, n: i32, a: &mut [Self], lda: i32, info: &mut i32
     );
 }
 
-macro_rules! impl_blas_xpotrf{
-    ($T:ty, $XPOTRF:path) => {
+pub trait XpotrsScalar: Sized {
+    fn xpotrs(
+        uplo: u8, n: i32, nrhs: i32, a: &[Self], lda: i32,  b: &mut [Self], ldb: i32, info: &mut i32
+    );
+}
+
+macro_rules! impl_blas_xpotrfs{
+    ($T:ty, $XPOTRF:path, $XPOTRS:path) => {
         impl XpotrfScalar for $T {
             fn xpotrf(
                 uplo: u8, n: i32, a: &mut [Self], lda: i32, info: &mut i32
             ) {
                 unsafe{
                     $XPOTRF(
                         uplo, n, a, lda, info
                     );
                 }
             }
         }
+        impl XpotrsScalar for $T {
+            fn xpotrs(
+                uplo: u8, n: i32, nrhs: i32, a: &[Self], lda: i32, b: &mut [Self], ldb: i32, info: &mut i32
+            ) {
+                unsafe{
+                    $XPOTRS(
+                        uplo, n, nrhs, a, lda, b, ldb, info
+                    );
+                }
+            }
+        }
     };
 }
 
 cfg_if::cfg_if! {
   if #[cfg(not(feature="sdp-r"))] {
       // R blas/lapack only provides double precision routines
-      impl_blas_xpotrf!(f32, spotrf);      
+      impl_blas_xpotrfs!(f32, spotrf, spotrs);      
   }
 }
-impl_blas_xpotrf!(f64, dpotrf);
+impl_blas_xpotrfs!(f64, dpotrf, dpotrs);
 
 
 // --------------------------------------
 // ?gesdd : SVD (divide and conquer method)
 // --------------------------------------
 
 pub trait XgesddScalar: Sized {
@@ -386,7 +402,44 @@
 cfg_if::cfg_if! {
   if #[cfg(not(feature="sdp-r"))] {
       // R blas/lapack only provides double precision routines
       impl_blas_gsyr2k!(f32, ssyr2k);
   }
 }
 impl_blas_gsyr2k!(f64, dsyr2k);
+
+
+// --------------------------------------
+// ?gesv : Generalized (LU) linear solve, multiple right hand side
+// --------------------------------------
+
+pub trait XgesvScalar: Sized {
+    fn xgesv(
+        n: i32, nrhs: i32, a: &mut [Self], lda: i32, ipiv: &mut [i32], 
+                b: &mut [Self], ldb: i32, info:&mut i32,
+    );
+}
+
+macro_rules! impl_blas_xgesv{
+    ($T:ty, $XGESV:path) => {
+        impl XgesvScalar for $T {
+            fn xgesv(
+                n: i32, nrhs: i32, a: &mut [Self], lda: i32, ipiv: &mut [i32], 
+                b: &mut [Self], ldb: i32, info:&mut i32,
+            ) {
+                unsafe{
+                    $XGESV(
+                        n, nrhs, a, lda, ipiv, b, ldb, info,
+                    );
+                }
+            }
+        }
+    };
+}
+
+cfg_if::cfg_if! {
+  if #[cfg(not(feature="sdp-r"))] {
+      // R blas/lapack only provides double precision routines
+      impl_blas_xgesv!(f32, sgesv);
+  }
+}
+impl_blas_xgesv!(f64, dgesv);
```

### Comparing `clarabel-0.7.1/src/algebra/dense/cholesky.rs` & `clarabel-0.8.0/src/algebra/dense/blas/cholesky.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,100 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{
-    DenseFactorizationError, FactorCholesky, FloatT, Matrix, MatrixTriangle, ShapedMatrix,
-    VectorMath,
-};
+use crate::algebra::*;
 
 pub(crate) struct CholeskyEngine<T> {
     /// lower triangular factor (stored as square dense)
     pub L: Matrix<T>,
 }
 
 impl<T> CholeskyEngine<T>
 where
     T: FloatT,
 {
     pub fn new(n: usize) -> Self {
         let L = Matrix::<T>::zeros((n, n));
         Self { L }
     }
+
+    pub fn resize(&mut self, n: usize) {
+        self.L.resize((n, n));
+    }
 }
 
-impl<T> FactorCholesky for CholeskyEngine<T>
+impl<T> FactorCholesky<T> for CholeskyEngine<T>
 where
     T: FloatT,
 {
-    type T = T;
-    fn cholesky(&mut self, A: &mut Matrix<Self::T>) -> Result<(), DenseFactorizationError> {
+    fn factor<S>(&mut self, A: &mut DenseStorageMatrix<S, T>) -> Result<(), DenseFactorizationError>
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
         if A.size() != self.L.size() {
             return Err(DenseFactorizationError::IncompatibleDimension);
         }
 
+        // ?potrf factors in place, so first copy A onto
+        // our internal factor matrix L.  We reference the
+        // upper triangle of A, but want a lower triangular
+        // result.  LAPACK factors triu inputs to U^TU, and
+        // tril inputs to LL^T, so first copy the triu part
+        // of A into tril of L before we factor it
+        let At = A.t();
+        let n = self.L.nrows();
+        for j in 0..n {
+            for i in j..n {
+                self.L[(i, j)] = At[(i, j)];
+            }
+        }
+
         // standard BLAS ?potrf arguments for computing
         // cholesky decomposition
-        let uplo = MatrixTriangle::Triu.as_blas_char(); // only look at triu of A
-        let An = A.nrows().try_into().unwrap();
-        let a = A.data_mut();
+        let uplo = MatrixTriangle::Tril.as_blas_char();
+        let An = self.L.nrows().try_into().unwrap();
+        let a = self.L.data_mut();
         let lda = An;
         let info = &mut 0_i32; // output info
 
         T::xpotrf(uplo, An, a, lda, info);
 
         if *info != 0 {
             return Err(DenseFactorizationError::Cholesky(*info));
         }
 
         // A will now have L^T in its upper triangle.
-        let At = A.t();
-        self.L.data_mut().set(T::zero());
-
-        let n = self.L.nrows();
-        for j in 0..n {
-            for i in j..n {
-                self.L[(i, j)] = At[(i, j)];
-            }
-        }
 
         Ok(())
     }
 
+    fn solve<S>(&mut self, B: &mut DenseStorageMatrix<S, T>)
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
+        // standard BLAS ?potrs arguments for computing
+        // post factorization triangular solve
+
+        // Tril here since we transposed A into L before
+        // factoring it
+        let uplo = MatrixTriangle::Tril.as_blas_char();
+
+        let nrhs = B.ncols().try_into().unwrap();
+        let An = self.L.nrows().try_into().unwrap();
+        let a = &self.L.data;
+        let lda = An;
+        let Bn = B.nrows().try_into().unwrap();
+        let b = B.data_mut();
+        let ldb = Bn;
+        let info = &mut 0_i32; // output info
+
+        T::xpotrs(uplo, An, nrhs, a, lda, b, ldb, info);
+
+        assert_eq!(*info, 0);
+    }
+
     fn logdet(&self) -> T {
         let mut ld = T::zero();
         let n = self.L.nrows();
         for i in 0..n {
             ld += T::ln(self.L[(i, i)]);
         }
         ld + ld
@@ -77,28 +110,44 @@
         &[[ 8., -2., 4.],
           [-2., 12., 2.],
           [ 4.,  2., 6.]]);
 
     let Scopy = S.clone(); //S is corrupted after factorization
 
     let mut eng = CholeskyEngine::<f64>::new(3);
-    assert!(eng.cholesky(&mut S).is_ok());
+    assert!(eng.factor(&mut S).is_ok());
 
     let mut M = Matrix::<f64>::zeros((3, 3));
     M.mul(&eng.L, &eng.L.t(), 1.0, 0.0);
 
     assert!(M.data().norm_inf_diff(Scopy.data()) < 1e-8);
+
+    // now try to solve with multiple RHS
+    let X = Matrix::from(&[
+        [1., 2.], //
+        [3., 4.], //
+        [5., 6.],
+    ]);
+    let mut B = Matrix::from(&[
+        [22., 32.], //
+        [44., 56.], //
+        [40., 52.],
+    ]);
+
+    eng.solve(&mut B);
+
+    assert!(B.data.norm_inf_diff(X.data()) <= 1e-14);
 }
 
 #[test]
 fn test_cholesky_logdet() {
     #[rustfmt::skip]
     let mut S = Matrix::from(
         &[[ 8., -2., 4.],
           [-2., 12., 2.],
           [ 4.,  2., 6.]]);
 
     let mut eng = CholeskyEngine::<f64>::new(3);
-    assert!(eng.cholesky(&mut S).is_ok());
+    assert!(eng.factor(&mut S).is_ok());
 
     assert!((eng.logdet() - 5.69035945432406).abs() < 1e-10);
 }
```

### Comparing `clarabel-0.7.1/src/algebra/dense/core.rs` & `clarabel-0.8.0/src/solver/implementations/default/variables.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,366 +1,290 @@
-#![allow(non_snake_case)]
+use super::*;
 use crate::algebra::*;
-use std::ops::{Index, IndexMut};
+use crate::solver::core::{
+    cones::{CompositeCone, Cone, PrimalOrDualCone},
+    traits::{Settings, Variables},
+    ScalingStrategy, StepDirection,
+};
+
+// ---------------
+// Variables type for default problem format
+// ---------------
+
+/// Standard-form solver type implementing the [`Variables`](crate::solver::core::traits::Variables) trait
+pub struct DefaultVariables<T> {
+    /// scaled primal variables
+    pub x: Vec<T>,
+    /// slack variables
+    pub s: Vec<T>,
+    /// scaled dual variables
+    pub z: Vec<T>,
+    /// homogenization scalar τ
+    pub τ: T,
+    /// homogenization scalar κ
+    pub κ: T,
+}
+
+impl<T: std::fmt::Display + std::fmt::Debug> std::fmt::Debug for DefaultVariables<T> {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(
+            f,
+            "x: {:?}\ns: {:?}\nz: {:?}\nτ: {:?}\nκ: {:?}\n",
+            self.x, self.s, self.z, self.τ, self.κ
+        )
+    }
+}
+
+impl<T> DefaultVariables<T>
+where
+    T: FloatT,
+{
+    pub fn new(n: usize, m: usize) -> Self {
+        let x = vec![T::zero(); n];
+        let s = vec![T::zero(); m];
+        let z = vec![T::zero(); m];
+        let τ = T::one();
+        let κ = T::one();
+
+        Self { x, s, z, τ, κ }
+    }
+}
+
+impl<T> Variables<T> for DefaultVariables<T>
+where
+    T: FloatT,
+{
+    type D = DefaultProblemData<T>;
+    type R = DefaultResiduals<T>;
+    type C = CompositeCone<T>;
+    type SE = DefaultSettings<T>;
+
+    fn calc_mu(&mut self, residuals: &DefaultResiduals<T>, cones: &CompositeCone<T>) -> T {
+        let denom = T::from(cones.degree() + 1).unwrap();
+        (residuals.dot_sz + self.τ * self.κ) / denom
+    }
+
+    fn affine_step_rhs(
+        &mut self,
+        residuals: &DefaultResiduals<T>,
+        variables: &Self,
+        cones: &CompositeCone<T>,
+    ) {
+        self.x.copy_from(&residuals.rx);
+        self.z.copy_from(&residuals.rz);
+        cones.affine_ds(&mut self.s, &variables.s);
+        self.τ = residuals.rτ;
+        self.κ = variables.τ * variables.κ;
+    }
+
+    fn combined_step_rhs(
+        &mut self,
+        residuals: &DefaultResiduals<T>,
+        variables: &Self,
+        cones: &mut CompositeCone<T>,
+        step: &mut Self,
+        σ: T,
+        μ: T,
+        m: T,
+    ) {
+        let dotσμ = σ * μ;
+
+        self.x.axpby(T::one() - σ, &residuals.rx, T::zero()); //self.x  = (1 - σ)*rx
+        self.τ = (T::one() - σ) * residuals.rτ;
+        self.κ = -dotσμ + m * step.τ * step.κ + variables.τ * variables.κ;
+
+        // ds is different for symmetric and asymmetric cones:
+        // Symmetric cones: d.s = λ ◦ λ + W⁻¹Δs ∘ WΔz − σμe
+        // Asymmetric cones: d.s = s + σμ*g(z)
+
+        // we want to scale the Mehotra correction in the symmetric
+        // case by M, so just scale step_z by M.  This is an unnecessary
+        // vector operation (since it amounts to M*z'*s), but it
+        // doesn't happen very often
+        if m != T::one() {
+            step.z.scale(m);
+        }
 
-/// Dense matrix in column major format
-///
-/// __Example usage__ : To construct the 3 x 3 matrix
-/// ```text
-/// A = [1.  3.  5.]
-///     [2.  0.  6.]
-///     [0.  4.  7.]
-/// ```
-///
-/// ```no_run
-/// use clarabel::algebra::Matrix;
-///
-/// let A : Matrix<f64> = Matrix::new(
-///    (3, 3),  //size as tuple
-///    vec![1., 2., 0., 3., 0., 4., 5., 6., 7.]
-///  );
-///
-/// ```
-
-#[derive(Debug, Clone, PartialEq)]
-pub struct Matrix<T = f64> {
-    /// number of rows
-    pub m: usize,
-    ///number of columns
-    pub n: usize,
-    /// vector of data in column major formmat
-    pub data: Vec<T>,
-}
+        cones.combined_ds_shift(&mut self.z, &mut step.z, &mut step.s, dotσμ);
 
-/// Creates a Matrix from a slice of arrays.
-///
-/// Example:
-/// ```
-/// use clarabel::algebra::Matrix;
-/// let A = Matrix::from(
-///      &[[1.0, 2.0],
-///        [3.0, 0.0],
-///        [0.0, 4.0]]);
-// ```
-//
-#[allow(clippy::needless_range_loop)]
-impl<'a, I, J, T> From<I> for Matrix<T>
-where
-    I: IntoIterator<Item = J>,
-    J: IntoIterator<Item = &'a T>,
-    T: FloatT,
-{
-    fn from(rows: I) -> Matrix<T> {
-        let rows: Vec<Vec<T>> = rows
-            .into_iter()
-            .map(|r| r.into_iter().copied().collect())
-            .collect();
-
-        let m = rows.len();
-        let n = rows.iter().map(|r| r.len()).next().unwrap_or(0);
-        assert!(rows.iter().all(|r| r.len() == n));
-        let nnz = m * n;
-
-        let mut data = Vec::with_capacity(nnz);
-        for c in 0..n {
-            for r in 0..m {
-                data.push(rows[r][c]);
-            }
-        }
+        //We are relying on d.s = affine_ds already here
+        self.s.axpby(T::one(), &self.z, T::one());
 
-        Matrix::<T> { m, n, data }
+        // now we copy the scaled res for rz and d.z is no longer work
+        self.z.axpby(T::one() - σ, &residuals.rz, T::zero());
     }
-}
 
-impl<T> Matrix<T>
-where
-    T: FloatT,
-{
-    pub fn zeros(size: (usize, usize)) -> Self {
-        let (m, n) = size;
-        let data = vec![T::zero(); m * n];
-        Self { m, n, data }
-    }
-
-    pub fn identity(n: usize) -> Self {
-        let mut mat = Matrix::zeros((n, n));
-        mat.set_identity();
-        mat
-    }
-
-    pub fn set_identity(&mut self) {
-        assert!(self.m == self.n);
-        self.data_mut().set(T::zero());
-        for i in 0..self.n {
-            self[(i, i)] = T::one();
-        }
-    }
+    fn calc_step_length(
+        &self,
+        step: &Self,
+        cones: &mut CompositeCone<T>,
+        settings: &DefaultSettings<T>,
+        step_direction: StepDirection,
+    ) -> T {
+        let ατ = {
+            if step.τ < T::zero() {
+                -self.τ / step.τ
+            } else {
+                T::max_value()
+            }
+        };
 
-    pub fn new(size: (usize, usize), data: Vec<T>) -> Self {
-        let (m, n) = size;
-        assert!(m * n == data.len());
-        Self { m, n, data }
-    }
+        let ακ = {
+            if step.κ < T::zero() {
+                -self.κ / step.κ
+            } else {
+                T::max_value()
+            }
+        };
 
-    pub fn new_from_slice(size: (usize, usize), src: &[T]) -> Self {
-        Self::new(size, src.to_vec())
-    }
+        let α = [ατ, ακ, T::one()].minimum();
+        let (αz, αs) = cones.step_length(&step.z, &step.s, &self.z, &self.s, settings.core(), α);
 
-    pub fn copy_from_slice(&mut self, src: &[T]) -> &mut Self {
-        self.data.copy_from_slice(src);
-        self
-    }
+        // itself only allows for a single maximum value.
+        // To enable split lengths, we need to also pass a
+        // tuple of limits to the step_length function of
+        // every cone
+        let mut α = T::min(αz, αs);
 
-    pub fn data_mut(&mut self) -> &mut [T] {
-        &mut self.data
-    }
+        if step_direction == StepDirection::Combined {
+            α *= settings.core().max_step_fraction;
+        }
 
-    pub fn t(&self) -> Adjoint<'_, Self> {
-        Adjoint { src: self }
+        α
     }
 
-    /// Returns a Symmetric view of a triu matrix
-    pub fn sym(&self) -> Symmetric<'_, Self> {
-        debug_assert!(self.is_triu());
-        Symmetric { src: self }
+    fn add_step(&mut self, step: &Self, α: T) {
+        self.x.axpby(α, &step.x, T::one());
+        self.s.axpby(α, &step.s, T::one());
+        self.z.axpby(α, &step.z, T::one());
+        self.τ += α * step.τ;
+        self.κ += α * step.κ;
     }
 
-    /// Set A = (A + A') / 2.  Assumes A is real
-    pub fn symmetric_part(&mut self) -> &mut Self {
-        assert!(self.is_square());
-        let half: T = (0.5_f64).as_T();
+    fn symmetric_initialization(&mut self, cones: &mut CompositeCone<T>) {
+        _shift_to_cone_interior(&mut self.s, cones, PrimalOrDualCone::PrimalCone);
+        _shift_to_cone_interior(&mut self.z, cones, PrimalOrDualCone::DualCone);
 
-        for r in 0..self.m {
-            for c in 0..r {
-                let val = half * (self[(r, c)] + self[(c, r)]);
-                self[(c, r)] = val;
-                self[(r, c)] = val;
-            }
-        }
-        self
+        self.τ = T::one();
+        self.κ = T::one();
     }
 
-    pub fn col_slice(&self, col: usize) -> &[T] {
-        assert!(col < self.n);
-        &self.data[(col * self.m)..(col + 1) * self.m]
-    }
+    fn unit_initialization(&mut self, cones: &CompositeCone<T>) {
+        cones.unit_initialization(&mut self.z, &mut self.s);
 
-    pub fn col_slice_mut(&mut self, col: usize) -> &mut [T] {
-        assert!(col < self.n);
-        &mut self.data[(col * self.m)..(col + 1) * self.m]
+        self.x.set(T::zero());
+        self.τ = T::one();
+        self.κ = T::one();
     }
 
-    pub fn is_triu(&self) -> bool {
-        for c in 0..self.ncols() {
-            for r in (c + 1)..self.nrows() {
-                if self[(r, c)] != T::zero() {
-                    return false;
-                }
-            }
-        }
-        true
+    fn copy_from(&mut self, src: &Self) {
+        self.x.copy_from(&src.x);
+        self.s.copy_from(&src.s);
+        self.z.copy_from(&src.z);
+        self.τ = src.τ;
+        self.κ = src.κ;
     }
-}
 
-impl<T> DenseMatrix for Matrix<T>
-where
-    T: FloatT,
-{
-    type T = T;
-    fn index_linear(&self, idx: (usize, usize)) -> usize {
-        idx.0 + self.m * idx.1
-    }
-    fn data(&self) -> &[T] {
-        &self.data
+    fn scale_cones(
+        &self,
+        cones: &mut CompositeCone<T>,
+        μ: T,
+        scaling_strategy: ScalingStrategy,
+    ) -> bool {
+        cones.update_scaling(&self.s, &self.z, μ, scaling_strategy)
     }
-}
 
-impl<'a, T> DenseMatrix for ReshapedMatrix<'a, T>
-where
-    T: FloatT,
-{
-    type T = T;
-    fn index_linear(&self, idx: (usize, usize)) -> usize {
-        idx.0 + self.m * idx.1
-    }
-    fn data(&self) -> &[T] {
-        self.data
-    }
-}
+    fn barrier(&self, step: &Self, α: T, cones: &mut CompositeCone<T>) -> T {
+        let central_coef = (cones.degree() + 1).as_T();
 
-impl<'a, T> DenseMatrix for Adjoint<'a, Matrix<T>>
-where
-    T: FloatT,
-{
-    type T = T;
-    #[inline]
-    fn index_linear(&self, idx: (usize, usize)) -> usize {
-        self.src.index_linear((idx.1, idx.0))
-    }
-    fn data(&self) -> &[T] {
-        &self.src.data
-    }
-}
+        let cur_τ = self.τ + α * step.τ;
+        let cur_κ = self.κ + α * step.κ;
 
-impl<'a, T> DenseMatrix for Symmetric<'a, Matrix<T>>
-where
-    T: FloatT,
-{
-    type T = T;
-    #[inline]
-    fn index_linear(&self, idx: (usize, usize)) -> usize {
-        if idx.0 <= idx.1 {
-            //triu part
-            self.src.index_linear((idx.0, idx.1))
-        } else {
-            //tril part uses triu entry
-            self.src.index_linear((idx.1, idx.0))
-        }
-    }
-    fn data(&self) -> &[T] {
-        &self.src.data
-    }
-}
+        // compute current μ
+        let sz = <[T] as VectorMath<T>>::dot_shifted(&self.z, &self.s, &step.z, &step.s, α);
+        let μ = (sz + cur_τ * cur_κ) / central_coef;
 
-impl<'a, T> ReshapedMatrix<'a, T>
-where
-    T: FloatT,
-{
-    pub fn from_slice(data: &'a [T], m: usize, n: usize) -> Self {
-        Self { data, m, n }
-    }
+        // barrier terms from gap and scalars
+        let mut barrier = central_coef * μ.logsafe() - cur_τ.logsafe() - cur_κ.logsafe();
 
-    #[allow(dead_code)]
-    pub fn reshape(&mut self, size: (usize, usize)) -> &Self {
-        assert!(size.0 * size.1 == self.m * self.n);
-        self.m = size.0;
-        self.n = size.1;
-        self
-    }
-}
+        // barriers from the cones
+        let (z, s) = (&self.z, &self.s);
+        let (dz, ds) = (&step.z, &step.s);
 
-impl<T> IndexMut<(usize, usize)> for Matrix<T>
-where
-    T: FloatT,
-{
-    fn index_mut(&mut self, idx: (usize, usize)) -> &mut Self::Output {
-        let lidx = self.index_linear(idx);
-        &mut self.data[lidx]
+        barrier += cones.compute_barrier(z, s, dz, ds, α);
+
+        barrier
     }
-}
 
-macro_rules! impl_mat_index {
-    ($mat:ty) => {
-        impl<T: FloatT> Index<(usize, usize)> for $mat {
-            type Output = T;
-            fn index(&self, idx: (usize, usize)) -> &Self::Output {
-                &self.data()[self.index_linear(idx)]
-            }
-        }
-    };
-}
-impl_mat_index!(Matrix<T>);
-impl_mat_index!(ReshapedMatrix<'_, T>);
-impl_mat_index!(Adjoint<'_, Matrix<T>>);
-impl_mat_index!(Symmetric<'_, Matrix<T>>);
+    fn rescale(&mut self) {
+        let scale = T::max(self.τ, self.κ);
+        let invscale = scale.recip();
 
-impl<T> ShapedMatrix for Matrix<T>
-where
-    T: FloatT,
-{
-    fn nrows(&self) -> usize {
-        self.m
-    }
-    fn ncols(&self) -> usize {
-        self.n
-    }
-    fn shape(&self) -> MatrixShape {
-        MatrixShape::N
+        self.x.scale(invscale);
+        self.z.scale(invscale);
+        self.s.scale(invscale);
+        self.τ *= invscale;
+        self.κ *= invscale;
     }
 }
 
-impl<T> Symmetric<'_, Matrix<T>>
+fn _shift_to_cone_interior<T>(z: &mut [T], cones: &mut CompositeCone<T>, pd: PrimalOrDualCone)
 where
     T: FloatT,
 {
-    pub(crate) fn pack_triu(&self, v: &mut [T]) {
-        let n = self.ncols();
-        let numel = triangular_number(n);
-        assert!(v.len() == numel);
-
-        let mut k = 0;
-        for col in 0..self.ncols() {
-            for row in 0..=col {
-                v[k] = self.src[(row, col)];
-                k += 1;
-            }
-        }
-    }
-}
+    let (min_margin, pos_margin) = cones.margins(z, pd);
+    let target = T::max(
+        T::one(),
+        (pos_margin * (0.1).as_T()) / cones.degree().as_T(),
+    );
 
-impl<T> std::fmt::Display for Matrix<T>
-where
-    T: FloatT,
-{
-    fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
-        _display_matrix(self, f)
+    if min_margin <= T::zero() {
+        // at least some component is outside its cone
+        // done in two stages since otherwise (1-α) = -α for
+        // large α, which makes z exactly 0. (or worse, -0.0 )
+        cones.scaled_unit_shift(z, -min_margin, pd);
+        cones.scaled_unit_shift(z, target, pd);
+    } else if min_margin < target {
+        // margin is positive but small.
+        cones.scaled_unit_shift(z, target - min_margin, pd);
+    } else {
+        // good margin, but still shift explicitly by
+        // zero to catch any elements in the zero cone
+        // that need to be forced to zero
+        cones.scaled_unit_shift(z, T::zero(), pd);
     }
 }
 
-fn _display_matrix<M>(m: &M, f: &mut std::fmt::Formatter) -> std::fmt::Result
+impl<T> DefaultVariables<T>
 where
-    M: DenseMatrix,
-    M::Output: FloatT,
+    T: FloatT,
 {
-    writeln!(f)?;
-    for i in 0..m.nrows() {
-        write!(f, "[ ")?;
-        for j in 0..m.ncols() {
-            write!(f, " {:?}", m[(i, j)])?;
-        }
-        writeln!(f, "]")?;
-    }
-    writeln!(f)?;
-    Ok(())
-}
-
-#[test]
-#[rustfmt::skip]
-fn test_matrix_istriu() {
-    
-    let A = Matrix::from(&[
-        [1., 2., 3.], 
-        [0., 2., 0.], 
-        [0., 0., 1.]]); 
-
-    assert_eq!(A.is_triu(),true);
-
-    let A = Matrix::from(&[
-        [1., 2., 3.], 
-        [0., 2., 0.], 
-        [1., 0., 1.]]); 
+    pub(crate) fn unscale(&mut self, data: &DefaultProblemData<T>, is_infeasible: bool) {
+        // if we have an infeasible problem, normalize
+        // using κ to get an infeasibility certificate.
+        // Otherwise use τ to get an unscaled solution.
+        let scaleinv = {
+            if is_infeasible {
+                T::recip(self.κ)
+            } else {
+                T::recip(self.τ)
+            }
+        };
 
-    assert_eq!(A.is_triu(),false);
-}
+        // also undo the equilibration
+        let d = &data.equilibration.d;
+        let (e, einv) = (&data.equilibration.e, &data.equilibration.einv);
+        let cscale = data.equilibration.c;
 
-#[test]
-#[rustfmt::skip]
-fn test_matrix_from_slice_of_arrays() {
-    let A = Matrix::new(
-        (3, 2), // n
-        vec![1., 3., 0., 2., 0., 4.],
-    );
+        self.x.hadamard(d).scale(scaleinv);
+        self.z.hadamard(e).scale(scaleinv / cscale);
+        self.s.hadamard(einv).scale(scaleinv);
 
-    let B = Matrix::from(&[
-        [1., 2.], 
-        [3., 0.], 
-        [0., 4.]]); 
-
-    let C: Matrix = (&[
-        [1., 2.], 
-        [3., 0.], 
-        [0., 4.],
-    ]).into();
+        self.τ *= scaleinv;
+        self.κ *= scaleinv;
+    }
 
-    assert_eq!(A, B);
-    assert_eq!(A, C);
+    #[cfg_attr(not(sdp), allow(dead_code))]
+    pub(crate) fn dims(&self) -> (usize, usize) {
+        (self.x.len(), self.s.len())
+    }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clarabel-0.7.1/src/algebra/dense/gemm.rs` & `clarabel-0.8.0/src/algebra/dense/blas/gemm.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{DenseMatrix, FloatT, Matrix, MatrixShape, MultiplyGEMM, ShapedMatrix};
+use crate::algebra::*;
 
-impl<T> MultiplyGEMM for Matrix<T>
+impl<S, T> MultiplyGEMM<T> for DenseStorageMatrix<S, T>
 where
     T: FloatT,
+    S: AsRef<[T]> + AsMut<[T]>,
 {
-    type T = T;
     // implements self = C = αA*B + βC
     fn mul<MATA, MATB>(&mut self, A: &MATA, B: &MATB, α: T, β: T) -> &Self
     where
-        MATA: DenseMatrix<T = T>,
-        MATB: DenseMatrix<T = T>,
+        MATA: DenseMatrix<T>,
+        MATB: DenseMatrix<T>,
     {
         assert!(A.ncols() == B.nrows() && self.nrows() == A.nrows() && self.ncols() == B.ncols());
 
         if self.nrows() == 0 || self.ncols() == 0 {
             return self;
         }
```

### Comparing `clarabel-0.7.1/src/algebra/dense/gemv.rs` & `clarabel-0.8.0/src/algebra/dense/blas/gemv.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #![allow(non_snake_case)]
 
 use crate::algebra::{
-    Adjoint, DenseMatrix, FloatT, Matrix, MatrixShape, MultiplyGEMV, ShapedMatrix,
+    Adjoint, DenseMatrix, DenseStorageMatrix, FloatT, Matrix, MatrixShape, MultiplyGEMV,
+    ShapedMatrix,
 };
 
-impl<T> MultiplyGEMV for Matrix<T>
+// PJG: This needs to be over generic storage
+impl<S, T> MultiplyGEMV<T> for DenseStorageMatrix<S, T>
 where
     T: FloatT,
+    S: AsRef<[T]>,
 {
-    type T = T;
     // implements y = αA*x + βy
-    fn gemv(&self, x: &[Self::T], y: &mut [Self::T], α: Self::T, β: Self::T) {
+    fn gemv(&self, x: &[T], y: &mut [T], α: T, β: T) {
         let (m, n) = self.size();
         Matrix::<T>::_gemv(self.shape(), m, n, α, self.data(), x, β, y);
     }
 }
 
-impl<'a, T> MultiplyGEMV for Adjoint<'a, Matrix<T>>
+impl<'a, S, T> MultiplyGEMV<T> for Adjoint<'a, DenseStorageMatrix<S, T>>
 where
     T: FloatT,
+    S: AsRef<[T]>,
 {
-    type T = T;
     // implements y = αA'*x + βy
-    fn gemv(&self, x: &[Self::T], y: &mut [Self::T], α: Self::T, β: Self::T) {
+    fn gemv(&self, x: &[T], y: &mut [T], α: T, β: T) {
         let (m, n) = self.src.size(); //NB: size of A, not A'
         Matrix::<T>::_gemv(self.shape(), m, n, α, self.data(), x, β, y);
     }
 }
 
 impl<T> Matrix<T>
 where
```

### Comparing `clarabel-0.7.1/src/algebra/dense/kron.rs` & `clarabel-0.8.0/src/algebra/dense/kron.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #![allow(non_snake_case)]
-use crate::algebra::{DenseMatrix, FloatT, Matrix, ShapedMatrix};
+use crate::algebra::*;
 
 impl<T> Matrix<T>
 where
     T: FloatT,
 {
-    pub(crate) fn kron<MATA, MATB>(&mut self, A: &MATA, B: &MATB) -> &Self
+    #[allow(dead_code)]
+    pub(crate) fn kron<MATA, MATB>(&mut self, A: &MATA, B: &MATB)
     where
-        MATB: DenseMatrix<T = T, Output = T>,
-        MATA: DenseMatrix<T = T, Output = T>,
+        MATA: DenseMatrix<T>,
+        MATB: DenseMatrix<T>,
     {
         let (pp, qq) = A.size();
         let (rr, ss) = B.size();
         assert!(self.nrows() == pp * rr);
         assert!(self.ncols() == qq * ss);
 
         let mut i = 0;
         for q in 0..qq {
             for s in 0..ss {
                 for p in 0..pp {
                     let Apq = A[(p, q)];
                     for r in 0..rr {
-                        self.data_mut()[i] = Apq * B[(r, s)];
+                        self.data_mut()[i] = (Apq) * B[(r, s)];
                         i += 1;
                     }
                 }
             }
         }
-        self
     }
 }
 
 #[test]
 #[rustfmt::skip]
 fn test_kron() {
```

### Comparing `clarabel-0.7.1/src/algebra/dense/matrix_math.rs` & `clarabel-0.8.0/src/algebra/dense/matrix_math.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,77 @@
 #![allow(non_snake_case)]
-use crate::algebra::{FloatT, Matrix, MatrixMath, VectorMath};
+use crate::algebra::*;
 
-impl<T: FloatT> MatrixMath for Matrix<T> {
-    type T = T;
+impl<T: FloatT> MatrixMath<T> for Matrix<T> {
 
-    //scalar mut operations
-    fn scale(&mut self, c: T) {
-        self.data.scale(c);
+    fn col_sums(&self, sums: &mut [T]) {
+        assert_eq!(self.ncols(), sums.len());
+        for (col, sum) in sums.iter_mut().enumerate() {
+            *sum = self.col_slice(col).sum();
+        }
     }
 
-    fn negate(&mut self) {
-        self.data.negate();
+    fn row_sums(&self, sums: &mut [T]) {
+        assert_eq!(self.nrows(), sums.len());
+        sums.fill(T::zero());
+        for col in 0..self.ncols() {
+            let slice = self.col_slice(col);
+            for (row, &v) in slice.iter().enumerate() {
+                sums[row] += v;
+            }
+        }
     }
 
     fn col_norms(&self, norms: &mut [T]) {
         norms.fill(T::zero());
         self.col_norms_no_reset(norms);
     }
 
     fn col_norms_no_reset(&self, norms: &mut [T]) {
         for (i, norm) in norms.iter_mut().enumerate() {
             let colnorm = self.col_slice(i).norm_inf();
-            *norm = Self::T::max(*norm, colnorm);
+            *norm = T::max(*norm, colnorm);
         }
     }
 
     fn col_norms_sym(&self, norms: &mut [T]) {
         norms.fill(T::zero());
         self.col_norms_sym_no_reset(norms);
     }
 
     fn col_norms_sym_no_reset(&self, norms: &mut [T]) {
-        for c in 0..self.n {
+        for c in 0..self.ncols() {
             for r in 0..=c {
                 let tmp = self[(r, c)];
                 norms[r] = T::max(norms[r], tmp);
                 norms[c] = T::max(norms[c], tmp);
             }
         }
     }
 
     fn row_norms(&self, norms: &mut [T]) {
         norms.fill(T::zero());
         self.row_norms_no_reset(norms);
     }
 
     fn row_norms_no_reset(&self, norms: &mut [T]) {
-        for r in 0..self.m {
-            for c in 0..self.n {
+        for r in 0..self.nrows() {
+            for c in 0..self.ncols() {
                 norms[r] = T::max(norms[r], T::abs(self[(r, c)]))
             }
         }
     }
 
-    fn lscale(&mut self, l: &[T]) {
-        for col in 0..self.n {
-            self.col_slice_mut(col).hadamard(l);
-        }
-    }
-
-    fn rscale(&mut self, r: &[T]) {
-        for (col, val) in r.iter().enumerate() {
-            self.col_slice_mut(col).scale(*val);
-        }
-    }
-
-    fn lrscale(&mut self, l: &[T], r: &[T]) {
-        for i in 0..self.m {
-            for j in 0..self.n {
-                self[(i, j)] *= l[i] * r[j];
-            }
-        }
-    }
-
     // PJG: this should probably only be implemented as part of
     // some SymmetricMatrixMath trait.  Uses upper triangle only
     // and assumes that the rest is symmetric.
     fn quad_form(&self, y: &[T], x: &[T]) -> T {
-        assert_eq!(self.m, self.n);
+        assert!(self.is_square());
         let mut out = T::zero();
-        for col in 0..self.n {
+        for col in 0..self.ncols() {
             let mut tmp1 = T::zero();
             let mut tmp2 = T::zero();
             for row in 0..=col {
                 let Mv = self[(row, col)];
                 if row < col {
                     tmp1 += Mv * x[row];
                     tmp2 += Mv * y[row];
@@ -94,14 +82,116 @@
             }
             out += tmp1 * y[col] + tmp2 * x[col];
         }
         out
     }
 }
 
+impl<T: FloatT> MatrixMathMut<T> for Matrix<T> {
+
+    //scalar mut operations
+    fn scale(&mut self, c: T) {
+        self.data.scale(c);
+    }
+
+    fn negate(&mut self) {
+        self.data.negate();
+    }
+
+    fn lscale(&mut self, l: &[T]) {
+        for col in 0..self.ncols() {
+            self.col_slice_mut(col).hadamard(l);
+        }
+    }
+
+    fn rscale(&mut self, r: &[T]) {
+        for (col, val) in r.iter().enumerate() {
+            self.col_slice_mut(col).scale(*val);
+        }
+    }
+
+    fn lrscale(&mut self, l: &[T], r: &[T]) {
+        for i in 0..self.nrows() {
+            for j in 0..self.ncols() {
+                self[(i, j)] *= l[i] * r[j];
+            }
+        }
+    }
+
+}
+
+
+// additional functions that require floating point operations
+
+// allow dead code here since dense matrix and its supporting
+// functionality could eventually become a public interface.
+#[allow(dead_code)]
+impl<S,T> DenseStorageMatrix<S, T> 
+where 
+    T: FloatT,
+    S: AsRef<[T]> + AsMut<[T]>
+{
+    /// Set A = (A + A') / 2.  Assumes A is real
+    pub fn symmetric_part(&mut self) -> &mut Self {
+        assert!(self.is_square());
+        let half: T = (0.5_f64).as_T();
+
+        for r in 0..self.nrows() {
+            for c in 0..r {
+                let val = half * (self[(r, c)] + self[(c, r)]);
+                self[(c, r)] = val;
+                self[(r, c)] = val;
+            }
+        }
+        self
+    }
+}
+
+
+pub(crate) fn svec_to_mat<S,T>(M: &mut DenseStorageMatrix<S,T>, x: &[T]) 
+where
+    T: FloatT,
+    S: AsRef<[T]> + AsMut<[T]>,
+{
+    let mut idx = 0;
+    for col in 0..M.ncols() {
+        for row in 0..=col {
+            if row == col {
+                M[(row, col)] = x[idx];
+            } else {
+                M[(row, col)] = x[idx] * T::FRAC_1_SQRT_2();
+                M[(col, row)] = x[idx] * T::FRAC_1_SQRT_2();
+            }
+            idx += 1;
+        }
+    }
+}
+
+//PJG : Perhaps implementation for Symmetric type would be faster
+pub(crate) fn mat_to_svec<T,MATM>(x: &mut [T], M: &MATM)
+where 
+MATM: DenseMatrix<T>,
+     T: FloatT,
+{
+    let mut idx = 0;
+    for col in 0..M.ncols() {
+        for row in 0..=col {
+            x[idx] = {
+                if row == col {
+                    M[(row, col)]
+                } else {
+                    (M[(row, col)] + M[(col, row)]) * T::FRAC_1_SQRT_2()
+                }
+            };
+            idx += 1;
+        }
+    }
+}
+
+
 #[test]
 fn test_quad_form() {
     let mut A = Matrix::from(&[
         [1., 4.], //
         [4., 5.], //
     ]);
 
@@ -112,22 +202,30 @@
     //remove lower triangle part and check again.
     //should not change the result.
     A[(1, 0)] = 0.0;
     assert!(A.quad_form(&x, &y) == 83.0);
 }
 
 #[test]
-fn test_row_col_norms() {
+fn test_row_col_sums_and_norms() {
     #[rustfmt::skip]
     let A = Matrix::from(&[
         [-1.,  4.,  6.], 
         [ 3., -8.,  7.], 
         [ 0.,  4.,  9.],
     ]);
 
+    let mut rsums = vec![0.0; 3];
+    let mut csums = vec![0.0; 3];
+
+    A.row_sums(&mut rsums);
+    assert_eq!(rsums, [9.0, 2.0, 13.0]);
+    A.col_sums(&mut csums);
+    assert_eq!(csums, [2.0, 0.0, 22.0]);
+
     let mut rnorms = vec![0.0; 3];
     let mut cnorms = vec![0.0; 3];
 
     A.row_norms(&mut rnorms);
     assert!(rnorms == [6.0, 8.0, 9.0]);
     A.col_norms(&mut cnorms);
     assert!(cnorms == [3.0, 8.0, 9.0]);
@@ -174,15 +272,15 @@
         [-1.,  4.,   6.], 
         [-6., 16., -14.], 
         [ 0., 12.,  27.],
     ]);
     assert_eq!(B,Btest);
 
     //left-right scale
-    let mut B = A.clone();
+    let mut B = A;
     B.lrscale(&lscale, &rscale);
     let Btest = Matrix::from(&[
         [ 2.,  4., -18.], 
         [12., 16.,  42.], 
         [ 0., 12., -81.],
     ]);
     assert_eq!(B,Btest);
```

### Comparing `clarabel-0.7.1/src/algebra/dense/svd.rs` & `clarabel-0.8.0/src/algebra/dense/blas/svd.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{DenseFactorizationError, FactorSVD, FloatT, Matrix, ShapedMatrix};
+use crate::algebra::*;
 use core::cmp::min;
+use std::iter::zip;
 
 #[derive(PartialEq, Eq)]
 #[allow(dead_code)] //QRDecomposition is not used yet
 pub(crate) enum SVDEngineAlgorithm {
     DivideAndConquer,
     QRDecomposition,
 }
@@ -47,22 +48,31 @@
             U,
             Vt,
             work,
             iwork,
             algorithm,
         }
     }
+
+    pub fn resize(&mut self, size: (usize, usize)) {
+        let (m, n) = size;
+        self.s.resize(min(m, n), T::zero());
+        self.U.resize((m, min(m, n)));
+        self.Vt.resize((min(m, n), n));
+    }
 }
 
-impl<T> FactorSVD for SVDEngine<T>
+impl<T> FactorSVD<T> for SVDEngine<T>
 where
     T: FloatT,
 {
-    type T = T;
-    fn svd(&mut self, A: &mut Matrix<Self::T>) -> Result<(), DenseFactorizationError> {
+    fn factor<S>(&mut self, A: &mut DenseStorageMatrix<S, T>) -> Result<(), DenseFactorizationError>
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
         let (m, n) = A.size();
 
         if self.U.nrows() != m || self.Vt.ncols() != n {
             return Err(DenseFactorizationError::IncompatibleDimension);
         }
 
         // standard BLAS ?gesdd and/or ?gesvd arguments for economy size SVD.
@@ -108,29 +118,84 @@
             if i == 0 {
                 lwork = work[0].to_i32().unwrap();
                 work.resize(lwork as usize, T::zero());
             }
         }
         Ok(())
     }
+
+    fn solve<S>(&mut self, B: &mut DenseStorageMatrix<S, T>)
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
+        // get the dimensions for the SVD factors
+        let m = self.U.nrows();
+        let n = self.Vt.ncols();
+        let k = min(m, n); //number of singular values
+
+        // this function only implemented for square matrices
+        // because otherwise writing the solution in place
+        // does not make sense.   This is not a good general
+        // implementation, but is only needed at present for a
+        // rank-deficient, symmetric square solves in PSD
+        // completion
+        assert_eq!(m, n);
+
+        // the number of columns in B
+        let nrhs = B.ncols();
+        assert_eq!(B.nrows(), m);
+
+        // compute a tolerance for the singular values
+        // to be considered invertible
+        let tol = T::epsilon() * self.s[0].abs() * T::from(k).unwrap();
+
+        // will compute B <- Vt * (Σ^-1 * (U^T * B))
+        // we need a workspace that is at least nrhs * k
+        // to hold the product C = U^T * B.  Will also
+        // allocate additional space to hold the inverted
+        // singular values
+        let work = &mut self.work;
+        work.resize(k + k * nrhs, T::zero());
+        let (sinv, workC) = work.split_at_mut(k);
+
+        // C <- U^T * B
+        let mut C = BorrowedMatrixMut::from_slice_mut(workC, k, nrhs);
+        C.mul(&self.U.t(), B, T::one(), T::zero());
+
+        // C <- Σ^-1 * C
+        zip(sinv.iter_mut(), self.s.iter()).for_each(|(sinv, s)| {
+            if s.abs() > tol {
+                *sinv = T::recip(s.abs());
+            } else {
+                *sinv = T::zero();
+            }
+        });
+
+        for col in 0..nrhs {
+            C.col_slice_mut(col).hadamard(sinv);
+        }
+
+        // B <- V * C
+        B.mul(&self.Vt.t(), &C, T::one(), T::zero());
+    }
 }
 
 #[test]
-fn test_svd() {
+fn test_svd_factor() {
     use crate::algebra::{DenseMatrix, MultiplyGEMM, VectorMath};
 
     let mut A = Matrix::from(&[
         [3., 2., 2.],  //
         [2., 3., -2.], //
     ]);
 
     let Acopy = A.clone(); //A is corrupted after factorization
 
     let mut eng = SVDEngine::<f64>::new((2, 3));
-    assert!(eng.svd(&mut A).is_ok());
+    assert!(eng.factor(&mut A).is_ok());
     let sol = [5., 3.];
     assert!(eng.s.norm_inf_diff(&sol) < 1e-8);
 
     let mut M = Matrix::<f64>::zeros((2, 3));
 
     let U = &eng.U;
     let s = &eng.s;
@@ -140,10 +205,42 @@
     let mut Us = U.clone();
     for c in 0..Us.ncols() {
         for r in 0..Us.nrows() {
             Us[(r, c)] *= s[c];
         }
     }
     M.mul(&Us, Vt, 1.0, 0.0);
-
     assert!(M.data().norm_inf_diff(Acopy.data()) < 1e-8);
 }
+
+#[test]
+fn test_svd_solve() {
+    use crate::algebra::{DenseMatrix, VectorMath};
+
+    // Singular and non-square A
+    let mut A = Matrix::from(&[
+        [2., 4., 6.], //
+        [1., 2., 3.], //
+        [0., 1., 2.],
+    ]);
+
+    let mut B = Matrix::from(&[
+        [1., 2.], //
+        [3., 4.],
+        [5., 6.],
+    ]);
+
+    // this appears to be an exact solution
+    let mut X = Matrix::from(&[
+        [-175., -200.], //
+        [-40., -44.],
+        [95., 112.],
+    ]);
+    X.data.scale(1. / 30.);
+
+    let mut eng = SVDEngine::<f64>::new((3, 3));
+
+    assert!(eng.factor(&mut A).is_ok());
+
+    eng.solve(&mut B);
+    assert!(B.data().norm_inf_diff(X.data()) < 1e-14);
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clarabel-0.7.1/src/algebra/dense/syevr.rs` & `clarabel-0.8.0/src/algebra/dense/blas/syevr.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{
-    DenseFactorizationError, FactorEigen, FloatT, Matrix, MatrixTriangle, ShapedMatrix,
-};
+use crate::algebra::*;
 
 pub(crate) struct EigEngine<T> {
     /// Computed eigenvalues in ascending order
     pub λ: Vec<T>,
 
     /// Computed eigenvectors (optional)
     pub V: Option<Matrix<T>>,
@@ -33,32 +31,47 @@
             isuppz,
             work,
             iwork,
         }
     }
 }
 
-impl<T> FactorEigen for EigEngine<T>
+impl<T> FactorEigen<T> for EigEngine<T>
 where
     T: FloatT,
 {
-    type T = T;
-    fn eigvals(&mut self, A: &mut Matrix<Self::T>) -> Result<(), DenseFactorizationError> {
+    fn eigvals<S>(
+        &mut self,
+        A: &mut DenseStorageMatrix<S, T>,
+    ) -> Result<(), DenseFactorizationError>
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
         self.syevr(A, b'N')
     }
-    fn eigen(&mut self, A: &mut Matrix<Self::T>) -> Result<(), DenseFactorizationError> {
+    fn eigen<S>(&mut self, A: &mut DenseStorageMatrix<S, T>) -> Result<(), DenseFactorizationError>
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
         self.syevr(A, b'V')
     }
 }
 
 impl<T> EigEngine<T>
 where
     T: FloatT,
 {
-    fn syevr(&mut self, A: &mut Matrix<T>, jobz: u8) -> Result<(), DenseFactorizationError> {
+    fn syevr<S>(
+        &mut self,
+        A: &mut DenseStorageMatrix<S, T>,
+        jobz: u8,
+    ) -> Result<(), DenseFactorizationError>
+    where
+        S: AsMut<[T]> + AsRef<[T]>,
+    {
         if !A.is_square() || A.nrows() != self.λ.len() {
             return Err(DenseFactorizationError::IncompatibleDimension);
         }
         let An = A.nrows();
 
         // allocate for eigenvectors on first request
         if jobz == b'V' && self.V.is_none() {
```

### Comparing `clarabel-0.7.1/src/algebra/dense/symv.rs` & `clarabel-0.8.0/src/algebra/dense/blas/symv.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/algebra/dense/syr2k.rs` & `clarabel-0.8.0/src/algebra/dense/blas/syr2k.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{
-    DenseMatrix, FloatT, Matrix, MatrixShape, MatrixTriangle, MultiplySYR2K, ShapedMatrix,
-};
+use crate::algebra::*;
 
-impl<T> MultiplySYR2K for Matrix<T>
+impl<S, T> MultiplySYR2K<T> for DenseStorageMatrix<S, T>
 where
     T: FloatT,
+    S: AsMut<[T]> + AsRef<[T]>,
 {
-    type T = T;
-
     // implements self = C = α(A*B' + B*A') + βC
-    fn syr2k(&mut self, A: &Matrix<T>, B: &Matrix<T>, α: T, β: T) -> &Self {
+    fn syr2k<S1, S2>(
+        &mut self,
+        A: &DenseStorageMatrix<S1, T>,
+        B: &DenseStorageMatrix<S2, T>,
+        α: T,
+        β: T,
+    ) where
+        S1: AsRef<[T]>,
+        S2: AsRef<[T]>,
+    {
         assert!(self.nrows() == A.nrows());
         assert!(self.nrows() == B.nrows());
         assert!(self.ncols() == B.nrows());
         assert!(A.ncols() == B.ncols());
 
         if self.nrows() == 0 {
-            return self;
+            return;
         }
 
         let n = self.nrows().try_into().unwrap();
         let k = A.ncols().try_into().unwrap();
         let a = A.data();
         let lda = n;
         let b = B.data();
@@ -40,15 +46,14 @@
             lda,
             b,
             ldb,
             β,
             c,
             ldc,
         );
-        self
     }
 }
 
 #[test]
 #[rustfmt::skip]
 fn test_syr2k() {
```

### Comparing `clarabel-0.7.1/src/algebra/dense/syrk.rs` & `clarabel-0.8.0/src/algebra/dense/blas/syrk.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #![allow(non_snake_case)]
 
-use crate::algebra::{
-    DenseMatrix, FloatT, Matrix, MatrixShape, MatrixTriangle, MultiplySYRK, ShapedMatrix,
-};
+use crate::algebra::*;
 
-impl<T> MultiplySYRK for Matrix<T>
+impl<T> MultiplySYRK<T> for Matrix<T>
 where
     T: FloatT,
 {
-    type T = T;
-
     // implements self = C = αA*A' + βC
-    fn syrk<MATA>(&mut self, A: &MATA, α: T, β: T) -> &Self
+    // The matrix input A can itself be
+    // an Adjoint matrix, in which case the
+    // result amounts to C = αA'*A + βC
+    fn syrk<MATA>(&mut self, A: &MATA, α: T, β: T)
     where
-        MATA: DenseMatrix<T = T>,
+        MATA: DenseMatrix<T>,
     {
         assert!(self.nrows() == A.nrows());
         assert!(self.ncols() == A.nrows());
 
         if self.nrows() == 0 {
-            return self;
+            return;
         }
 
         let uplo = MatrixTriangle::Triu.as_blas_char();
         let transA = A.shape().as_blas_char();
         let n = A.nrows().try_into().unwrap();
         let k = A.ncols().try_into().unwrap();
         let lda = if A.shape() == MatrixShape::N { n } else { k };
@@ -37,15 +36,14 @@
             α,
             A.data(),
             lda,
             β,
             self.data_mut(),
             ldc,
         );
-        self
     }
 }
 
 #[test]
 fn test_syrk() {
     let (m, n) = (2, 3);
     let A = Matrix::from(&[
```

### Comparing `clarabel-0.7.1/src/algebra/densesym3x3/mod.rs` & `clarabel-0.8.0/src/algebra/densesym3x3/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #![allow(non_snake_case)]
 
-use super::FloatT;
 use crate::algebra::*;
 use std::ops::{Index, IndexMut};
 
 // 3x3 Dense matrix types are restricted to the crate
 // NB: Implements a symmetric 3x3 type to support
 // power and exponential cones.
 //
```

### Comparing `clarabel-0.7.1/src/algebra/error_types.rs` & `clarabel-0.8.0/src/algebra/error_types.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 use thiserror::Error;
 
-/// Error type returned by sparse matrix user input checkers, e.g. [`check_format`](crate::algebra::CscMatrix::check_format) utility.
+/// Error type returned by matrix concatenation operations.
 #[derive(Error, Debug)]
+pub enum MatrixConcatenationError {
+    #[error("Incompatible dimensions")]
+    IncompatibleDimension,
+}
+
+#[derive(Error, Debug)]
+/// Error type returned by sparse matrix assembly operations.
 pub enum SparseFormatError {
     #[error("Matrix dimension fields and/or array lengths are incompatible")]
     IncompatibleDimension,
     #[error("Data is not sorted by row index within each column")]
     BadRowOrdering,
     #[error("Row value exceeds the matrix row dimension")]
     BadRowval,
@@ -13,18 +20,22 @@
     BadColptr,
     #[error("sparsity pattern mismatch")]
     SparsityMismatch,
 }
 
 /// Error type returned by BLAS-like dense factorization routines.  Errors
 /// return the internal BLAS error codes.
+#[allow(clippy::upper_case_acronyms)]
+#[allow(dead_code)]
 #[derive(Error, Debug)]
-pub enum DenseFactorizationError {
+pub(crate) enum DenseFactorizationError {
     #[error("Matrix dimension fields and/or array lengths are incompatible")]
     IncompatibleDimension,
     #[error("Eigendecomposition error")]
     Eigen(i32),
     #[error("SVD error")]
     SVD(i32),
     #[error("Cholesky error")]
     Cholesky(i32),
+    #[error("LU error")]
+    LU(i32),
 }
```

### Comparing `clarabel-0.7.1/src/algebra/floats.rs` & `clarabel-0.8.0/src/algebra/floats.rs`

 * *Files 10% similar despite different names*

```diff
@@ -40,42 +40,60 @@
 {
 }
 
 // if "sdp" is enabled, we must add an additional trait
 // trait bound to restrict compilation for f32/f64 types
 // since there is no BLAS support otherwise
 
+// Define the documentation string as a macro so that FloatT gets documentation
+// regardless of whether the "sdp" feature is enabled.
+macro_rules! floatT_doc_header {
+    () => {
+        r#"Main trait for floating point types used in the Clarabel solver."#
+    };
+}
+macro_rules! floatT_doc_long {
+    () => {
+        r#"All floating point calculations in Clarabel are represented internally on values 
+         implementing the `FloatT` trait, with implementations provided only for f32 and f64 
+         native types when compiled with BLAS/LAPACK support for SDPs. If SDP support is not 
+         enabled then it should be possible to compile Clarabel to support any any other 
+         floating point type provided that it satisfies the trait bounds of `CoreFloatT`. 
+        \
+        \
+         `FloatT` relies on [`num_traits`](num_traits) for most of its constituent trait bounds."#
+    };
+}
 cfg_if::cfg_if! {
     if #[cfg(not(feature="sdp"))] {
-    /// Main trait for floating point types used in the Clarabel solver.
-    ///
-    /// All floating point calculations in Clarabel are represented internally on values
-    /// implementing the `FloatT` trait, with implementations provided only for f32 and f64
-    /// native types when compiled with BLAS/LAPACK support for SDPs. If SDP support is not
-    /// enabled then it should be possible to compile Clarabel to support any any other
-    /// floating point type provided that it satisfies the trait bounds of `CoreFloatT`.
+    #[doc = floatT_doc_header!()]
     ///
-    /// `FloatT` relies on [`num_traits`](num_traits) for most of its constituent trait bounds.
+    #[doc = floatT_doc_long!()]
         pub trait FloatT: CoreFloatT {}
     } else{
+        #[doc = floatT_doc_header!()]
+        ///
+        #[doc = floatT_doc_long!()]
+        ///
+        /// The trait bound `BlasFloatT` is only enforced when compiling with the `sdp` feature.
         pub trait FloatT: CoreFloatT + BlasFloatT {}
     }
 }
 
 cfg_if::cfg_if! {
     if #[cfg(feature="sdp")] {
         impl<T> FloatT for T where T: CoreFloatT + BlasFloatT {}
     } else{
         impl<T> FloatT for T where T: CoreFloatT {}
     }
 }
 
 /// Trait for convering Rust primitives to [`FloatT`](crate::algebra::FloatT)
 ///
-/// This convenience trait implemented on f32/64 and u32/64.  This trait
+/// This convenience trait is implemented on f32/64 and u32/64.  This trait
 /// is required internally by the solver for converting constant primitives
 /// to [`FloatT`](crate::algebra::FloatT).  It is also used by the
 /// [user settings](crate::solver::implementations::default::DefaultSettings)
 /// for converting defaults of primitive type to [`FloatT`](crate::algebra::FloatT).
 
 // NB: `AsFloatT` is a convenience trait for f32/64 and u32/64
 // so that we can do things like (2.0).as_T() everywhere on
```

### Comparing `clarabel-0.7.1/src/algebra/math_traits.rs` & `clarabel-0.8.0/src/algebra/math_traits.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,49 @@
-use super::FloatT;
-
 // All internal math for all solver implementations should go
 // through these core traits, which are implemented generically
 // for floats of type FloatT.
 
 /// Scalar operations on [`FloatT`](crate::algebra::FloatT)
 
 pub trait ScalarMath {
-    type T: FloatT;
     /// Applies a threshold value.   
     ///
     /// Restricts the value to be at least `min_thresh` and at most `max_thresh`.
-    fn clip(&self, min_thresh: Self::T, max_thresh: Self::T) -> Self::T;
+    fn clip(&self, min_thresh: Self, max_thresh: Self) -> Self;
 
     /// Safe calculation for log barriers.
     ///
     /// Returns log(s) if s > 0   -Infinity otherwise.
-    fn logsafe(&self) -> Self::T;
+    fn logsafe(&self) -> Self;
 }
 
 /// Vector operations on slices of [`FloatT`](crate::algebra::FloatT)
 
-pub trait VectorMath {
-    type T;
-
+pub trait VectorMath<T> {
     /// Copy values from `src` to `self`
     fn copy_from(&mut self, src: &Self) -> &mut Self;
 
     /// Make a new vector from a subset of elements
-    fn select(&self, index: &[bool]) -> Vec<Self::T>;
+    fn select(&self, index: &[bool]) -> Vec<T>;
 
     /// Apply an elementwise operation on a vector.
-    fn scalarop(&mut self, op: impl Fn(Self::T) -> Self::T) -> &mut Self;
+    fn scalarop(&mut self, op: impl Fn(T) -> T) -> &mut Self;
 
     /// Apply an elementwise operation to `v` and assign the
     /// results to `self`.
-    fn scalarop_from(&mut self, op: impl Fn(Self::T) -> Self::T, v: &Self) -> &mut Self;
+    fn scalarop_from(&mut self, op: impl Fn(T) -> T, v: &Self) -> &mut Self;
 
     /// Elementwise translation.
-    fn translate(&mut self, c: Self::T) -> &mut Self;
+    fn translate(&mut self, c: T) -> &mut Self;
 
     /// set all elements to the same value
-    fn set(&mut self, c: Self::T) -> &mut Self;
+    fn set(&mut self, c: T) -> &mut Self;
 
     /// Elementwise scaling.
-    fn scale(&mut self, c: Self::T) -> &mut Self;
+    fn scale(&mut self, c: T) -> &mut Self;
 
     /// Elementwise reciprocal.
     fn recip(&mut self) -> &mut Self;
 
     /// Elementwise square root.
     fn sqrt(&mut self) -> &mut Self;
 
@@ -58,149 +53,149 @@
     /// Elementwise negation of entries.
     fn negate(&mut self) -> &mut Self;
 
     /// Elementwise scaling by another vector. Produces `self[i] = self[i] * y[i]`
     fn hadamard(&mut self, y: &Self) -> &mut Self;
 
     /// Vector version of [clip](crate::algebra::ScalarMath::clip)
-    fn clip(&mut self, min_thresh: Self::T, max_thresh: Self::T) -> &mut Self;
+    fn clip(&mut self, min_thresh: T, max_thresh: T) -> &mut Self;
 
     /// Normalize, returning the norm.  Do nothing if norm == 0.  
-    fn normalize(&mut self) -> Self::T;
+    fn normalize(&mut self) -> T;
 
     /// Dot product
-    fn dot(&self, y: &Self) -> Self::T;
+    fn dot(&self, y: &Self) -> T;
 
     // computes dot(z + αdz,s + αds) without intermediate allocation
-    fn dot_shifted(
-        z: &[Self::T],
-        s: &[Self::T],
-        dz: &[Self::T],
-        ds: &[Self::T],
-        α: Self::T,
-    ) -> Self::T;
+    fn dot_shifted(z: &[T], s: &[T], dz: &[T], ds: &[T], α: T) -> T;
 
     /// Standard Euclidian or 2-norm distance from `self` to `y`
-    fn dist(&self, y: &Self) -> Self::T;
+    fn dist(&self, y: &Self) -> T;
 
     /// Sum of elements.
-    fn sum(&self) -> Self::T;
+    fn sum(&self) -> T;
 
     /// Sum of squares of the elements.
-    fn sumsq(&self) -> Self::T;
+    fn sumsq(&self) -> T;
 
     /// 2-norm
-    fn norm(&self) -> Self::T;
+    fn norm(&self) -> T;
 
     /// Infinity norm
-    fn norm_inf(&self) -> Self::T;
+    fn norm_inf(&self) -> T;
 
     /// One norm
-    fn norm_one(&self) -> Self::T;
+    fn norm_one(&self) -> T;
 
     /// 2-norm of an elementwise scaling of `self` by `v`
-    fn norm_scaled(&self, v: &Self) -> Self::T;
+    fn norm_scaled(&self, v: &Self) -> T;
 
     /// Inf-norm of an elementwise scaling of `self` by `v`
-    fn norm_inf_scaled(&self, v: &Self) -> Self::T;
+    fn norm_inf_scaled(&self, v: &Self) -> T;
 
     /// Inf-norm of an elementwise scaling of `self` by `v`
-    fn norm_one_scaled(&self, v: &Self) -> Self::T;
+    fn norm_one_scaled(&self, v: &Self) -> T;
 
     // Inf-norm of vector difference
-    fn norm_inf_diff(&self, b: &Self) -> Self::T;
+    fn norm_inf_diff(&self, b: &Self) -> T;
 
     /// Minimum value in vector
-    fn minimum(&self) -> Self::T;
+    fn minimum(&self) -> T;
 
     /// Maximum value in vector
-    fn maximum(&self) -> Self::T;
+    fn maximum(&self) -> T;
 
     /// Mean value in vector
-    fn mean(&self) -> Self::T;
+    fn mean(&self) -> T;
 
     /// Checks if all elements are finite, i.e. no Infs or NaNs
     fn is_finite(&self) -> bool;
 
     //blas-like vector ops
     //--------------------
 
     /// BLAS-like shift and scale in place.  Produces `self = a*x+b*self`
-    fn axpby(&mut self, a: Self::T, x: &Self, b: Self::T) -> &mut Self;
+    fn axpby(&mut self, a: T, x: &Self, b: T) -> &mut Self;
 
     /// BLAS-like shift and scale, non in-place version.  Produces `self = a*x+b*y`
-    fn waxpby(&mut self, a: Self::T, x: &Self, b: Self::T, y: &Self) -> &mut Self;
+    fn waxpby(&mut self, a: T, x: &Self, b: T, y: &Self) -> &mut Self;
 }
 
 /// Matrix operations for matrices of [`FloatT`](crate::algebra::FloatT)
 
-pub(crate) trait MatrixVectorMultiply {
-    type T: FloatT;
-
+pub(crate) trait MatrixVectorMultiply<T> {
     /// BLAS-like general matrix-vector multiply.  Produces `y = a*self*x + b*y`
-    fn gemv(&self, y: &mut [Self::T], x: &[Self::T], a: Self::T, b: Self::T);
+    fn gemv(&self, y: &mut [T], x: &[T], a: T, b: T);
 }
 
-pub(crate) trait SymMatrixVectorMultiply {
-    type T: FloatT;
-
+pub(crate) trait SymMatrixVectorMultiply<T> {
     /// BLAS-like symmetric matrix-vector multiply.  Produces `y = a*self*x + b*y`.  
     /// The matrix source data should be triu.
-    fn symv(&self, y: &mut [Self::T], x: &[Self::T], a: Self::T, b: Self::T);
+    fn symv(&self, y: &mut [T], x: &[T], a: T, b: T);
 }
 
 /// Operations on matrices of [`FloatT`](crate::algebra::FloatT)
 
-pub trait MatrixMath {
-    type T: FloatT;
+pub trait MatrixMath<T> {
+    /// Compute columnwise sums on a matrix and
+    /// assign the results to the vector `sums`
+    fn col_sums(&self, sums: &mut [T]);
+
+    /// Compute columnwise sums on a matrix and
+    /// assign the results to the vector `sums`
+    fn row_sums(&self, sums: &mut [T]);
 
     /// Compute columnwise infinity norm operations on
     /// a matrix and assign the results to the vector `norms`
-    fn col_norms(&self, norms: &mut [Self::T]);
+    fn col_norms(&self, norms: &mut [T]);
 
     /// Compute columnwise infinity norm operations on
     /// a matrix and assign the results to the vector `norms`.
     /// In the `no_reset` version of this function, if `norms[i]`
     /// is already larger the norm of the $i^{th}$ columns, then
     /// its value is not changed
-    fn col_norms_no_reset(&self, norms: &mut [Self::T]);
+    fn col_norms_no_reset(&self, norms: &mut [T]);
 
     /// Compute columnwise infinity norm operations on
     /// a symmstric matrix
-    fn col_norms_sym(&self, norms: &mut [Self::T]);
+    fn col_norms_sym(&self, norms: &mut [T]);
 
     /// Compute columnwise infinity norm operations on
     /// a symmetric matrix without reset
-    fn col_norms_sym_no_reset(&self, norms: &mut [Self::T]);
+    fn col_norms_sym_no_reset(&self, norms: &mut [T]);
 
     /// Compute rowwise infinity norm operations on
     /// a matrix and assign the results to the vector `norms`
-    fn row_norms(&self, norms: &mut [Self::T]);
+    fn row_norms(&self, norms: &mut [T]);
 
     /// Compute rowwise infinity norm operations on
     /// a matrix and assign the results to the vector `norms`
     /// without reset
-    fn row_norms_no_reset(&self, norms: &mut [Self::T]);
+    fn row_norms_no_reset(&self, norms: &mut [T]);
+
+    /// Quadratic form for a symmetric matrix.  Assumes that the
+    /// matrix `M = self` is in upper triangular form, and produces
+    /// `y^T*M*x`
+    ///
+    /// PJG: Maybe this should be on symmetric only.
+    fn quad_form(&self, y: &[T], x: &[T]) -> T;
+}
+
+/// Operations on mutable matrices of [`FloatT`](crate::algebra::FloatT)
 
+pub trait MatrixMathMut<T> {
     /// Elementwise scaling
-    fn scale(&mut self, c: Self::T);
+    fn scale(&mut self, c: T);
 
     /// Elementwise negation
     fn negate(&mut self);
 
     /// Left multiply the matrix `self` by `Diagonal(l)`
-    fn lscale(&mut self, l: &[Self::T]);
+    fn lscale(&mut self, l: &[T]);
 
     /// Right multiply the matrix self by `Diagonal(r)`
-    fn rscale(&mut self, r: &[Self::T]);
+    fn rscale(&mut self, r: &[T]);
 
     /// Left and multiply the matrix self by diagonal matrices,
     /// producing `A = Diagonal(l)*A*Diagonal(r)`
-    fn lrscale(&mut self, l: &[Self::T], r: &[Self::T]);
-
-    /// Quadratic form for a symmetric matrix.  Assumes that the
-    /// matrix `M = self` is in upper triangular form, and produces
-    /// `y^T*M*x`
-    ///
-    /// PJG: Maybe this should be on symmetric only.
-    fn quad_form(&self, y: &[Self::T], x: &[Self::T]) -> Self::T;
+    fn lrscale(&mut self, l: &[T], r: &[T]);
 }
```

### Comparing `clarabel-0.7.1/src/algebra/matrix_types.rs` & `clarabel-0.8.0/src/algebra/matrix_types.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-// All internal matrix representations in the default
-// solver and math implementations are in standard
-// compressed sparse column format, as is the API.
+use crate::algebra::ShapedMatrix;
 
 /// Matrix shape marker for triangular matrices
 #[derive(PartialEq, Eq, Copy, Clone)]
 pub enum MatrixTriangle {
     /// Upper triangular matrix
     Triu,
     /// Lower triangular matrix
     Tril,
 }
 
 /// Matrix triangular form marker
 impl MatrixTriangle {
     /// convert to u8 character for BLAS calls
+    #[cfg(feature = "sdp")]
     pub fn as_blas_char(&self) -> u8 {
         match self {
             MatrixTriangle::Triu => b'U',
             MatrixTriangle::Tril => b'L',
         }
     }
     /// transpose
+    #[allow(dead_code)]
     pub fn t(&self) -> Self {
         match self {
             MatrixTriangle::Triu => MatrixTriangle::Tril,
             MatrixTriangle::Tril => MatrixTriangle::Triu,
         }
     }
 }
@@ -36,44 +36,62 @@
     N,
     /// Transposed matrix orientation
     T,
 }
 
 impl MatrixShape {
     /// convert to u8 character for BLAS calls
+    #[cfg(feature = "sdp")]
     pub fn as_blas_char(&self) -> u8 {
         match self {
             MatrixShape::N => b'N',
             MatrixShape::T => b'T',
         }
     }
     /// transpose
+    #[allow(dead_code)]
     pub fn t(&self) -> Self {
         match self {
             MatrixShape::N => MatrixShape::T,
             MatrixShape::T => MatrixShape::N,
         }
     }
 }
 
+//-------------------------------------
+// Adjoint and Symmetric matrix views
+
 /// Adjoint of a matrix
 #[derive(Debug, Clone, PartialEq)]
 pub struct Adjoint<'a, M> {
     pub src: &'a M,
 }
 /// Symmetric view of a matrix.   Only the upper
 /// triangle of the source matrix will be referenced.
 #[derive(Debug, Clone, PartialEq)]
 pub struct Symmetric<'a, M> {
     pub src: &'a M,
 }
 
-/// Borrowed data slice reshaped into a matrix.
-#[derive(Debug, Clone, PartialEq)]
-pub(crate) struct ReshapedMatrix<'a, T> {
-    /// number of rows
-    pub m: usize,
-    ///number of columns
-    pub n: usize,
-    ///borrowed data
-    pub data: &'a [T],
+impl<'a, M> ShapedMatrix for Adjoint<'a, M>
+where
+    M: ShapedMatrix,
+{
+    fn size(&self) -> (usize, usize) {
+        (self.src.ncols(), self.src.nrows())
+    }
+    fn shape(&self) -> MatrixShape {
+        MatrixShape::T
+    }
+}
+
+impl<'a, M> ShapedMatrix for Symmetric<'a, M>
+where
+    M: ShapedMatrix,
+{
+    fn size(&self) -> (usize, usize) {
+        (self.src.ncols(), self.src.nrows())
+    }
+    fn shape(&self) -> MatrixShape {
+        MatrixShape::N
+    }
 }
```

### Comparing `clarabel-0.7.1/src/algebra/mod.rs` & `clarabel-0.8.0/src/algebra/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 //!
 //! All floating point calculations are represented internally on values implementing the
 //! [`FloatT`] trait.
 
 // first import and flatten the solver's collection
 // of core numeric types and matrix / vector traits.
 
-mod adjoint;
 mod error_types;
 mod floats;
 mod math_traits;
 mod matrix_traits;
 mod matrix_types;
-mod reshaped;
 mod scalarmath;
-mod symmetric;
+mod utils;
 mod vecmath;
-pub use adjoint::*;
 pub use error_types::*;
 pub use floats::*;
 pub use math_traits::*;
 pub use matrix_traits::*;
-pub use matrix_types::*;
-pub use reshaped::*;
+pub(crate) use matrix_types::*;
 pub(crate) use scalarmath::*;
-pub use symmetric::*;
-pub use vecmath::*;
+pub(crate) use utils::*;
 
 // matrix implementations
 mod csc;
 pub use csc::*;
 
 mod densesym3x3;
 pub(crate) use densesym3x3::*;
 
 #[cfg(feature = "sdp")]
 mod dense;
 #[cfg(feature = "sdp")]
-pub use dense::*;
+pub(crate) use dense::*;
+// sparse vectors implementations (for chordal decomp only)
+#[cfg(feature = "sdp")]
+mod sparsevector;
+#[cfg(feature = "sdp")]
+pub(crate) use sparsevector::*;
 
 //configure tests of internals
 #[cfg(test)]
 mod tests;
```

### Comparing `clarabel-0.7.1/src/algebra/tests/matrix.rs` & `clarabel-0.8.0/src/algebra/tests/matrix.rs`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,30 @@
     let mut A = test_matrix_4x4();
     //was Ai = vec![0, 2, 0, 1, 3, 0, 1, 2, 2, 3]
     A.rowval = vec![0, 2, 0, 1, 4, 0, 1, 2, 2, 3];
     assert!(A.check_format().is_err());
 }
 
 #[test]
+fn test_row_sums() {
+    let A = test_matrix_3x4();
+    let mut v = vec![0.0; 3];
+    A.row_sums(&mut v);
+    assert_eq!(v, vec![-2., 10., -9.]);
+}
+
+#[test]
+fn test_col_sums() {
+    let A = test_matrix_3x4();
+    let mut v = vec![0.0; 4];
+    A.col_sums(&mut v);
+    assert_eq!(v, vec![2., -21., 13., 5.]);
+}
+
+#[test]
 fn test_col_norms() {
     let A = test_matrix_3x4();
     let mut v = vec![0., -30., 12., 4.]; //big values should be ignored
     A.col_norms(&mut v);
     assert_eq!(v, vec![3., 17., 7., 10.]);
 
     let mut v = vec![0., -30., 12., 4.]; //big values should NOT be ignored
```

### Comparing `clarabel-0.7.1/src/algebra/tests/vector.rs` & `clarabel-0.8.0/src/algebra/tests/vector.rs`

 * *Files 25% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     let mut y = vec![0.; 4];
     y.copy_from(&x);
     assert_eq!(x, y);
 }
 
 #[test]
 fn test_select() {
-    let x = vec![1., 2., 3., 4., 5.];
-    let idx = vec![true, false, true, true, false];
+    let x = [1., 2., 3., 4., 5.];
+    let idx = [true, false, true, true, false];
     let y = x.select(&idx);
     assert_eq!(y, vec![1., 3., 4.]);
 }
 
 #[test]
 fn test_scalarop() {
     let mut x = vec![3., 0., 2., 1.];
@@ -29,29 +29,29 @@
     let mut y: Vec<f64> = vec![0.; 4];
     y.scalarop_from(|x| -2. * x, &x);
     assert_eq!(y, vec![-6., 0., -4., -2.]);
 }
 
 #[test]
 fn test_translate() {
-    let mut x = vec![3., 0., 2., 1.];
+    let mut x = [3., 0., 2., 1.];
     x.translate(-4.);
-    assert_eq!(x, vec![-1., -4., -2., -3.]);
+    assert_eq!(x, [-1., -4., -2., -3.]);
 }
 
 #[test]
 fn test_scale() {
-    let mut x = vec![3., 0., 2., 1.];
+    let mut x = [3., 0., 2., 1.];
     x.scale(3.);
-    assert_eq!(x, vec![9., 0., 6., 3.]);
+    assert_eq!(x, [9., 0., 6., 3.]);
 }
 
 #[test]
 fn test_recip() {
-    let mut x = vec![3., 10., 2., 1.];
+    let mut x = [3., 10., 2., 1.];
     x.recip();
     assert!(x.norm_inf_diff(&[1. / 3., 1. / 10., 1. / 2., 1.]) < 1e-8);
 }
 
 #[test]
 fn test_sqrt() {
     let mut x = vec![9., 4., 16., 0.];
@@ -115,58 +115,58 @@
 
     assert_eq!(x.dist(&y), f64::sqrt(30.));
     assert_eq!(y.dist(&x), f64::sqrt(30.));
 }
 
 #[test]
 fn test_sumsq() {
-    let x = vec![-1., 2., -3., 4.];
+    let x = [-1., 2., -3., 4.];
     assert_eq!(x.sumsq(), 30.);
 }
 
 #[test]
 fn test_norm() {
-    let x = vec![-3., 4., -12.];
+    let x = [-3., 4., -12.];
     assert_eq!(x.norm(), 13.);
 }
 
 #[test]
 fn test_norm_scaled() {
-    let x = vec![-3. / 2., 4. / 3., -12. / 4.];
-    let s = vec![2., 3., 4.];
+    let x = [-3. / 2., 4. / 3., -12. / 4.];
+    let s = [2., 3., 4.];
     assert_eq!(x.norm_scaled(&s), 13.);
 }
 
 #[test]
 fn test_norm_inf() {
-    let x = vec![-3., 4., -12.];
+    let x = [-3., 4., -12.];
     assert_eq!(x.norm_inf(), 12.);
 }
 
 #[test]
 fn test_norm_one() {
-    let x = vec![-3., 4., -12.];
+    let x = [-3., 4., -12.];
     assert_eq!(x.norm_one(), 19.);
 }
 
 #[test]
 fn test_minimum() {
-    let x = vec![-3., 4., -12.];
+    let x = [-3., 4., -12.];
     assert_eq!(x.minimum(), -12.);
 }
 
 #[test]
 fn test_maximum() {
-    let x = vec![-3., 4., -12.];
+    let x = [-3., 4., -12.];
     assert_eq!(x.maximum(), 4.);
 }
 
 #[test]
 fn test_mean() {
-    let x = vec![-3., 4., -12., -1.];
+    let x = [-3., 4., -12., -1.];
     assert_eq!(x.mean(), -3.);
 }
 
 #[test]
 fn test_axpby() {
     let x = vec![3., 0., 2., 1.];
     let mut y = vec![-1., -2., -1., 0.];
```

### Comparing `clarabel-0.7.1/src/algebra/vecmath.rs` & `clarabel-0.8.0/src/algebra/vecmath.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use super::{FloatT, ScalarMath, VectorMath};
 use itertools::izip;
 use std::iter::zip;
 
-impl<T: FloatT> VectorMath for [T] {
-    type T = T;
+impl<T: FloatT> VectorMath<T> for [T] {
     fn copy_from(&mut self, src: &[T]) -> &mut Self {
         self.copy_from_slice(src);
         self
     }
 
     fn select(&self, index: &[bool]) -> Vec<T> {
         assert_eq!(self.len(), index.len());
@@ -139,21 +138,21 @@
             let prod = x * y;
             acc + prod * prod
         });
         T::sqrt(total)
     }
 
     //inf-norm of elementwise product self.*v
-    fn norm_inf_scaled(&self, v: &Self) -> Self::T {
+    fn norm_inf_scaled(&self, v: &Self) -> T {
         assert_eq!(self.len(), v.len());
         zip(self, v).fold(T::zero(), |acc, (&x, &y)| T::max(acc, T::abs(x * y)))
     }
 
     //
-    fn norm_one_scaled(&self, v: &Self) -> Self::T {
+    fn norm_one_scaled(&self, v: &Self) -> T {
         zip(self, v).fold(T::zero(), |acc, (&x, &y)| acc + T::abs(x * y))
     }
 
     // max absolute difference (used for unit testing)
     fn norm_inf_diff(&self, b: &[T]) -> T {
         zip(self, b).fold(T::zero(), |acc, (x, y)| T::max(acc, T::abs(*x - *y)))
     }
```

### Comparing `clarabel-0.7.1/src/julia/ClarabelRs/src/ClarabelRs.jl` & `clarabel-0.8.0/src/julia/ClarabelRs/src/ClarabelRs.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/julia/ClarabelRs/src/interface.jl` & `clarabel-0.8.0/src/julia/ClarabelRs/src/interface.jl`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     P::SparseMatrixCSC{Float64,Int64},
     c::Vector{Float64},
     A::SparseMatrixCSC{Float64,Int64},
     b::Vector{Float64},
     cone_types::Vector{<:Clarabel.SupportedCone},
     settings::Clarabel.Settings{Float64}
 ) 
+    # protect against cones with overly specific type, e.g. 
+    # when all of the cones are NonnegativeConeT
+    cone_types = convert(Vector{Clarabel.SupportedCone},cone_types)
+
     s = solver_new_jlrs(P,c,A,b,cone_types,settings)
     return s
 end
 
 function solve!(solver::Solver)
 
     #this is the solution as a SolutionJLRS
@@ -98,16 +102,15 @@
 # -------------------------------------
 # functions for passing cones and settings 
 # -------------------------------------
 
 
 function ccall_cones_to_array(cones::Vector{Clarabel.SupportedCone})
 
-    rscones = ConeDataJLRS[]
-    sizehint!(rscones,length(cones))
+    rscones = sizehint!(ConeDataJLRS[],length(cones))
     
     for cone in cones
 
         rscone = begin 
             if isa(cone, Clarabel.ZeroConeT)
                 ConeDataJLRS(ZeroConeT::ConeEnumJLRS;
                     int = cone.dim,
```

### Comparing `clarabel-0.7.1/src/julia/ClarabelRs/src/types.jl` & `clarabel-0.8.0/src/julia/ClarabelRs/src/types.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl` & `clarabel-0.8.0/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # ============================ /test/MOI_wrapper.jl ============================
 # Test structure taken from https://jump.dev/JuMP.jl/stable/moi/submodules/Test/overview/
 
 module TestClarabelRs
 
-import ClarabelRs, Clarabel
+import ClarabelRs, Clarabel, JuMP
 using MathOptInterface
 using Test
 
 const MOI = MathOptInterface
 
 T = Float64
-optimizer = ClarabelRs.Optimizer()
-MOI.set(optimizer,MOI.Silent(),false)
-
-BRIDGED = MOI.Bridges.full_bridge_optimizer(
-    MOI.Utilities.CachingOptimizer(
-        MOI.Utilities.UniversalFallback(MOI.Utilities.Model{T}()),
-        optimizer,
-    ),
-    T,
+optimizer =  JuMP.optimizer_with_attributes(
+            ClarabelRs.Optimizer, 
+            "chordal_decomposition_enable" => true, 
+            "chordal_decomposition_merge_method" => :clique_graph,
+            "chordal_decomposition_compact" => true,
+            "chordal_decomposition_complete_dual" => true,
+       );
+
+const BRIDGED = MOI.instantiate(
+    optimizer,
+    with_bridge_type = Float64,
 )
 
+#
+
+
 # See the docstring of MOI.Test.Config for other arguments.
 MYCONFIG = MOI.Test.Config(
     # Modify tolerances as necessary.
     atol = 1e-4,
     rtol = 1e-4,
     # Use MOI.LOCALLY_SOLVED for local solvers.
     optimal_status = MOI.OPTIMAL,
```

### Comparing `clarabel-0.7.1/src/julia/ClarabelRs/test/test_jump.jl` & `clarabel-0.8.0/src/julia/ClarabelRs/test/test_jump.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/julia/README.md` & `clarabel-0.8.0/src/julia/README.md`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/julia/interface.rs` & `clarabel-0.8.0/src/julia/interface.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/julia/types.rs` & `clarabel-0.8.0/src/julia/types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/lib.rs` & `clarabel-0.8.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/.gitignore` & `clarabel-0.8.0/src/python/.gitignore`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/cones_py.rs` & `clarabel-0.8.0/src/python/cones_py.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/cscmatrix_py.rs` & `clarabel-0.8.0/src/python/cscmatrix_py.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-#![allow(unused)]
 #![allow(non_snake_case)]
 
 use crate::algebra::CscMatrix;
 use core::ops::Deref;
-use pyo3::exceptions::PyTypeError;
-use pyo3::{prelude::*, PyClass};
-use std::{cmp::Ordering, fmt::Write, io};
+use pyo3::prelude::*;
 
 //We can't implement the foreign trait FromPyObject directly on CscMatrix
 //since it is outside the crate, so put a dummy wrapper around it here.
 pub struct PyCscMatrix(CscMatrix<f64>);
 
 impl Deref for PyCscMatrix {
     type Target = CscMatrix<f64>;
@@ -24,15 +21,14 @@
 }
 
 impl<'a> FromPyObject<'a> for PyCscMatrix {
     fn extract(obj: &'a PyAny) -> PyResult<Self> {
         let nzval: Vec<f64> = obj.getattr("data")?.extract()?;
         let rowval: Vec<usize> = obj.getattr("indices")?.extract()?;
         let colptr: Vec<usize> = obj.getattr("indptr")?.extract()?;
-        let nnz: usize = obj.getattr("nnz")?.extract()?;
         let shape: Vec<usize> = obj.getattr("shape")?.extract()?;
 
         let mat = CscMatrix::new(shape[0], shape[1], colptr, rowval, nzval);
 
         Ok(PyCscMatrix(mat))
     }
 }
```

### Comparing `clarabel-0.7.1/src/python/impl_default_py.rs` & `clarabel-0.8.0/src/python/impl_default_py.rs`

 * *Files 9% similar despite different names*

```diff
@@ -243,14 +243,24 @@
     pub iterative_refinement_max_iter: u32,
     #[pyo3(get, set)]
     pub iterative_refinement_stop_ratio: f64,
 
     // preprocessing
     #[pyo3(get, set)]
     pub presolve_enable: bool,
+
+    //chordal decomposition (python must be built with "sdp" feature)
+    #[pyo3(get, set)]
+    pub chordal_decomposition_enable: bool,
+    #[pyo3(get, set)]
+    pub chordal_decomposition_merge_method: String,
+    #[pyo3(get, set)]
+    pub chordal_decomposition_compact: bool,
+    #[pyo3(get, set)]
+    pub chordal_decomposition_complete_dual: bool,
 }
 
 #[pymethods]
 impl PyDefaultSettings {
     #[new]
     pub fn new() -> Self {
         PyDefaultSettings::new_from_internal(&DefaultSettings::<f64>::default())
@@ -312,14 +322,18 @@
             dynamic_regularization_delta: set.dynamic_regularization_delta,
             iterative_refinement_enable: set.iterative_refinement_enable,
             iterative_refinement_reltol: set.iterative_refinement_reltol,
             iterative_refinement_abstol: set.iterative_refinement_abstol,
             iterative_refinement_max_iter: set.iterative_refinement_max_iter,
             iterative_refinement_stop_ratio: set.iterative_refinement_stop_ratio,
             presolve_enable: set.presolve_enable,
+            chordal_decomposition_enable: set.chordal_decomposition_enable,
+            chordal_decomposition_merge_method: set.chordal_decomposition_merge_method.clone(),
+            chordal_decomposition_compact: set.chordal_decomposition_compact,
+            chordal_decomposition_complete_dual: set.chordal_decomposition_complete_dual,
         }
     }
 
     pub(crate) fn to_internal(&self) -> DefaultSettings<f64> {
         // convert python settings -> Rust
 
         DefaultSettings::<f64> {
@@ -356,14 +370,18 @@
             dynamic_regularization_delta: self.dynamic_regularization_delta,
             iterative_refinement_enable: self.iterative_refinement_enable,
             iterative_refinement_reltol: self.iterative_refinement_reltol,
             iterative_refinement_abstol: self.iterative_refinement_abstol,
             iterative_refinement_max_iter: self.iterative_refinement_max_iter,
             iterative_refinement_stop_ratio: self.iterative_refinement_stop_ratio,
             presolve_enable: self.presolve_enable,
+            chordal_decomposition_enable: self.chordal_decomposition_enable,
+            chordal_decomposition_merge_method: self.chordal_decomposition_merge_method.clone(),
+            chordal_decomposition_compact: self.chordal_decomposition_compact,
+            chordal_decomposition_complete_dual: self.chordal_decomposition_complete_dual,
         }
     }
 }
 
 // ----------------------------------
 // Solver
 // ----------------------------------
```

### Comparing `clarabel-0.7.1/src/python/io.rs` & `clarabel-0.8.0/src/python/io.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/mod.rs` & `clarabel-0.8.0/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/module_py.rs` & `clarabel-0.8.0/src/python/module_py.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/pyblas/blas_loader.rs` & `clarabel-0.8.0/src/python/pyblas/blas_loader.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/pyblas/blas_types.rs` & `clarabel-0.8.0/src/python/pyblas/blas_types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/pyblas/blas_wrappers.rs` & `clarabel-0.8.0/src/python/pyblas/blas_wrappers.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/python/pyblas/lapack_loader.rs` & `clarabel-0.8.0/src/python/pyblas/lapack_loader.rs`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 
         unsafe {
             let ptrs = PyLapackPointers {
                 dsyevr_: get_ptr!(api, "dsyevr"),
                 ssyevr_: get_ptr!(api, "ssyevr"),
                 dpotrf_: get_ptr!(api, "dpotrf"),
                 spotrf_: get_ptr!(api, "spotrf"),
+                dpotrs_: get_ptr!(api, "dpotrs"),
+                spotrs_: get_ptr!(api, "spotrs"),
                 dgesdd_: get_ptr!(api, "dgesdd"),
                 sgesdd_: get_ptr!(api, "sgesdd"),
                 dgesvd_: get_ptr!(api, "dgesvd"),
                 sgesvd_: get_ptr!(api, "sgesvd"),
+                dgesv_: get_ptr!(api, "dgesv"),
+                sgesv_: get_ptr!(api, "sgesv"),
             };
             Ok(ptrs)
         }
     }
 }
```

### Comparing `clarabel-0.7.1/src/python/pyblas/lapack_types.rs` & `clarabel-0.8.0/src/python/pyblas/lapack_types.rs`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 use libc::{c_char, c_int};
 
 pub struct PyLapackPointers {
     pub dsyevr_: DSYEVR,
     pub ssyevr_: SSYEVR,
     pub dpotrf_: DPOTRF,
     pub spotrf_: SPOTRF,
+    pub dpotrs_: DPOTRS,
+    pub spotrs_: SPOTRS,
     pub dgesdd_: DGESDD,
     pub sgesdd_: SGESDD,
     pub dgesvd_: DGESVD,
     pub sgesvd_: SGESVD,
+    pub dgesv_: DGESV,
+    pub sgesv_: SGESV,
 }
 
 type DSYEVR = extern "C" fn(
     jobz: *const c_char,
     range: *const c_char,
     uplo: *const c_char,
     n: *const c_int,
@@ -72,14 +76,36 @@
     uplo: *const c_char,
     n: *const c_int,
     A: *mut f32,
     lda: *const c_int,
     info: *mut c_int,
 );
 
+type DPOTRS = extern "C" fn(
+    uplo: *const c_char,
+    n: *const c_int,
+    nrhs: *const c_int,
+    A: *const f64,
+    lda: *const c_int,
+    B: *mut f64,
+    ldb: *const c_int,
+    info: *mut c_int,
+);
+
+type SPOTRS = extern "C" fn(
+    uplo: *const c_char,
+    n: *const c_int,
+    nrhs: *const c_int,
+    A: *const f32,
+    lda: *const c_int,
+    B: *mut f32,
+    ldb: *const c_int,
+    info: *mut c_int,
+);
+
 type DGESDD = extern "C" fn(
     jobz: *const c_char,
     m: *const c_int,
     n: *const c_int,
     A: *mut f64,
     lda: *const c_int,
     S: *mut f64,
@@ -139,7 +165,29 @@
     ldu: *const c_int,
     VT: *mut f32,
     ldvt: *const c_int,
     work: *mut f32,
     lwork: *const c_int,
     info: *mut c_int,
 );
+
+type DGESV = extern "C" fn(
+    n: *const c_int,
+    nrhs: *const c_int,
+    A: *mut f64,
+    lda: *const c_int,
+    ipiv: *mut c_int,
+    B: *mut f64,
+    ldb: *const c_int,
+    info: *mut c_int,
+);
+
+type SGESV = extern "C" fn(
+    n: *const c_int,
+    nrhs: *const c_int,
+    A: *mut f32,
+    lda: *const c_int,
+    ipiv: *mut c_int,
+    B: *mut f32,
+    ldb: *const c_int,
+    info: *mut c_int,
+);
```

### Comparing `clarabel-0.7.1/src/python/pyblas/lapack_wrappers.rs` & `clarabel-0.8.0/src/python/pyblas/lapack_wrappers.rs`

 * *Files 15% similar despite different names*

```diff
@@ -116,14 +116,58 @@
     (PYLAPACK.dpotrf_)(&(uplo as c_char), &n, a.as_mut_ptr(), &lda, info)
 }
 
 pub unsafe fn spotrf(uplo: u8, n: i32, a: &mut [f32], lda: i32, info: &mut i32) {
     (PYLAPACK.spotrf_)(&(uplo as c_char), &n, a.as_mut_ptr(), &lda, info)
 }
 
+pub unsafe fn dpotrs(
+    uplo: u8,
+    n: i32,
+    nrhs: i32,
+    a: &[f64],
+    lda: i32,
+    b: &mut [f64],
+    ldb: i32,
+    info: &mut i32,
+) {
+    (PYLAPACK.dpotrs_)(
+        &(uplo as c_char),
+        &n,
+        &nrhs,
+        a.as_ptr(),
+        &lda,
+        b.as_mut_ptr(),
+        &ldb,
+        info,
+    )
+}
+
+pub unsafe fn spotrs(
+    uplo: u8,
+    n: i32,
+    nrhs: i32,
+    a: &[f32],
+    lda: i32,
+    b: &mut [f32],
+    ldb: i32,
+    info: &mut i32,
+) {
+    (PYLAPACK.spotrs_)(
+        &(uplo as c_char),
+        &n,
+        &nrhs,
+        a.as_ptr(),
+        &lda,
+        b.as_mut_ptr(),
+        &ldb,
+        info,
+    )
+}
+
 pub unsafe fn dgesdd(
     jobz: u8,
     m: i32,
     n: i32,
     a: &mut [f64],
     lda: i32,
     s: &mut [f64],
@@ -251,7 +295,51 @@
         vt.as_mut_ptr(),
         &ldvt,
         work.as_mut_ptr(),
         &lwork,
         info,
     )
 }
+
+pub unsafe fn dgesv(
+    n: i32,
+    nrhs: i32,
+    a: &mut [f64],
+    lda: i32,
+    ipiv: &mut [i32],
+    b: &mut [f64],
+    ldb: i32,
+    info: &mut i32,
+) {
+    (PYLAPACK.dgesv_)(
+        &n,
+        &nrhs,
+        a.as_mut_ptr(),
+        &lda,
+        ipiv.as_mut_ptr(),
+        b.as_mut_ptr(),
+        &ldb,
+        info,
+    )
+}
+
+pub unsafe fn sgesv(
+    n: i32,
+    nrhs: i32,
+    a: &mut [f32],
+    lda: i32,
+    ipiv: &mut [i32],
+    b: &mut [f32],
+    ldb: i32,
+    info: &mut i32,
+) {
+    (PYLAPACK.sgesv_)(
+        &n,
+        &nrhs,
+        a.as_mut_ptr(),
+        &lda,
+        ipiv.as_mut_ptr(),
+        b.as_mut_ptr(),
+        &ldb,
+        info,
+    )
+}
```

### Comparing `clarabel-0.7.1/src/python/pyblas/mod.rs` & `clarabel-0.8.0/src/python/pyblas/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/qdldl/qdldl.rs` & `clarabel-0.8.0/src/qdldl/qdldl.rs`

 * *Files 4% similar despite different names*

```diff
@@ -334,17 +334,17 @@
     L: &mut CscMatrix<T>,
     D: &mut [T],
     Dinv: &mut [T],
     workspace: &mut QDLDLWorkspace<T>,
     logical: bool,
 ) -> Result<(), QDLDLError> {
     if logical {
-        L.nzval.fill(T::zero());
-        D.fill(T::zero());
-        Dinv.fill(T::zero());
+        L.nzval.fill(T::one());
+        D.fill(T::one());
+        Dinv.fill(T::one());
     }
 
     // factor using QDLDL C style converted code
     let A = &workspace.triuA;
 
     let pos_d_count = _factor_inner(
         A.n,
@@ -564,17 +564,15 @@
                 let y_vals_cidx = y_vals[cidx];
 
                 let (f, l) = (Lp[cidx], tmp_idx);
                 unsafe {
                     //Safety : Here the Lij index comes from the rowval
                     //field of the sparse L factor matrix, and should
                     //always be bounded by the matrix dimension.
-                    for j in f..l {
-                        let Lxj = *Lx.get_unchecked(j);
-                        let Lij = *Li.get_unchecked(j);
+                    for (&Lxj, &Lij) in zip(&Lx[f..l], &Li[f..l]) {
                         *(y_vals.get_unchecked_mut(Lij)) -= Lxj * y_vals_cidx;
                     }
                 }
 
                 // Now I have the cidx^th element of y = L\b.
                 // so compute the corresponding element of
                 // this row of L and put it into the right place
@@ -657,33 +655,29 @@
 // Solves (L+I)x = b, with x replacing b.  Unchecked version
 fn _lsolve_unsafe<T: FloatT>(Lp: &[usize], Li: &[usize], Lx: &[T], x: &mut [T]) {
     unsafe {
         for i in 0..x.len() {
             let xi = *x.get_unchecked(i);
             let f = *Lp.get_unchecked(i);
             let l = *Lp.get_unchecked(i + 1);
-            for j in f..l {
-                let Lxj = *Lx.get_unchecked(j);
-                let Lij = *Li.get_unchecked(j);
+            for (&Lxj, &Lij) in zip(&Lx[f..l], &Li[f..l]) {
                 *(x.get_unchecked_mut(Lij)) -= Lxj * xi;
             }
         }
     }
 }
 
 // Solves (L+I)'x = b, with x replacing b.  Unchecked version.
 fn _ltsolve_unsafe<T: FloatT>(Lp: &[usize], Li: &[usize], Lx: &[T], x: &mut [T]) {
     unsafe {
         for i in (0..x.len()).rev() {
             let mut s = T::zero();
             let f = *Lp.get_unchecked(i);
             let l = *Lp.get_unchecked(i + 1);
-            for j in f..l {
-                let Lxj = *Lx.get_unchecked(j);
-                let Lij = *Li.get_unchecked(j);
+            for (&Lxj, &Lij) in zip(&Lx[f..l], &Li[f..l]) {
                 s += Lxj * (*x.get_unchecked(Lij));
             }
             *x.get_unchecked_mut(i) -= s;
         }
     }
 }
```

### Comparing `clarabel-0.7.1/src/qdldl/test.rs` & `clarabel-0.8.0/src/qdldl/test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use super::*;
-use crate::algebra::{CscMatrix, FloatT};
 extern crate amd;
 
 #[cfg(test)]
 
 fn test_matrix_4x4() -> CscMatrix<f64> {
     // A =
     //[ 8.0  -3.0   2.0    ⋅ ]
@@ -66,36 +65,36 @@
 fn test_solve_from_factors() {
     //L =
     //[ ⋅    ⋅     ⋅    ⋅ ]
     //[1.0   ⋅     ⋅    ⋅ ]
     //[2.0  1.0    ⋅    ⋅ ]
     //[ ⋅   7.0  -3.0   ⋅ ]
 
-    let Lp = vec![0, 2, 4, 5, 5];
-    let Li = vec![1, 2, 2, 3, 3];
-    let Lx = vec![1., 2., 1., 7., -3.];
-    let _d = vec![4., -1., -2., 1.];
+    let Lp = [0, 2, 4, 5, 5];
+    let Li = [1, 2, 2, 3, 3];
+    let Lx = [1., 2., 1., 7., -3.];
+    let _d = [4., -1., -2., 1.];
     let dinv = [0.25, -1.0, -0.5, 1.0];
-    let x = vec![-3., 2., 1., 4.];
+    let x = [-3., 2., 1., 4.];
 
     //(I+L)x = b.  Back solve on b in place.
-    let mut b = vec![-3., -1., -3., 15.];
+    let mut b = [-3., -1., -3., 15.];
     _lsolve_unsafe(&Lp, &Li, &Lx, &mut b);
     assert_eq!(b, x);
 
-    let mut b = vec![-3., -1., -3., 15.];
+    let mut b = [-3., -1., -3., 15.];
     _lsolve_safe(&Lp, &Li, &Lx, &mut b);
     assert_eq!(b, x);
 
     //(I+L')x = b.  Back solve on b in place.
-    let mut b = vec![1., 31., -11., 4.];
+    let mut b = [1., 31., -11., 4.];
     _ltsolve_unsafe(&Lp, &Li, &Lx, &mut b);
     assert_eq!(b, x);
 
-    let mut b = vec![1., 31., -11., 4.];
+    let mut b = [1., 31., -11., 4.];
     _ltsolve_safe(&Lp, &Li, &Lx, &mut b);
     assert_eq!(b, x);
 
     //(I+L)*D*(I+L)*x = b.  Back solve on b in place;
     let mut b = vec![4., -27., -1., -279.];
     _solve(&Lp, &Li, &Lx, &dinv, &mut b);
     assert_eq!(b, x);
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/compositecone.rs` & `clarabel-0.8.0/src/solver/core/cones/compositecone.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use super::*;
 use crate::algebra::triangular_number;
-use crate::solver::CoreSettings;
 use std::collections::HashMap;
 use std::iter::zip;
 use std::ops::Range;
 
 // -------------------------------------
 // default composite cone type
 // -------------------------------------
@@ -64,34 +63,34 @@
         }
 
         // count up elements and degree
         let numel = cones.iter().map(|c| c.numel()).sum();
         let degree = cones.iter().map(|c| c.degree()).sum();
 
         //ranges for the subvectors associated with each cone,
-        //and the rangse for with the corresponding entries
+        //and the ranges for the corresponding entries
         //in the Hs sparse block
 
-        let rng_cones = _make_rng_cones(&cones);
-        let rng_blocks = _make_rng_blocks(&cones);
+        let rng_cones = make_rng_cones(&cones);
+        let rng_blocks = make_rng_blocks(&cones);
 
         Self {
             cones,
             //types,
             type_counts,
             numel,
             degree,
             rng_cones,
             rng_blocks,
             _is_symmetric,
         }
     }
 }
 
-fn _make_rng_cones<T>(cones: &[SupportedCone<T>]) -> Vec<Range<usize>>
+fn make_rng_cones<T>(cones: &[SupportedCone<T>]) -> Vec<Range<usize>>
 where
     T: FloatT,
 {
     let mut rngs = Vec::with_capacity(cones.len());
 
     if !cones.is_empty() {
         let mut start = 0;
@@ -100,15 +99,15 @@
             rngs.push(start..stop);
             start = stop;
         }
     }
     rngs
 }
 
-fn _make_rng_blocks<T>(cones: &[SupportedCone<T>]) -> Vec<Range<usize>>
+fn make_rng_blocks<T>(cones: &[SupportedCone<T>]) -> Vec<Range<usize>>
 where
     T: FloatT,
 {
     let mut rngs = Vec::with_capacity(cones.len());
 
     if !cones.is_empty() {
         let mut start = 0;
@@ -124,27 +123,14 @@
             rngs.push(start..stop);
             start = stop;
         }
     }
     rngs
 }
 
-fn _make_headidx<T>(headidx: &mut [usize], cones: &[SupportedCone<T>])
-where
-    T: FloatT,
-{
-    if !cones.is_empty() {
-        // index of first element in each cone
-        headidx[0] = 0;
-        for i in 2..headidx.len() {
-            headidx[i] = headidx[i - 1] + cones[i - 1].numel();
-        }
-    }
-}
-
 impl<T> CompositeCone<T>
 where
     T: FloatT,
 {
     pub fn len(&self) -> usize {
         self.cones.len()
     }
@@ -317,42 +303,41 @@
         ds: &[T],
         z: &[T],
         s: &[T],
         settings: &CoreSettings<T>,
         αmax: T,
     ) -> (T, T) {
         let mut α = αmax;
+        let all_symmetric = self.is_symmetric();
 
-        // Force symmetric cones first.
-        for (cone, rng) in zip(&mut self.cones, &self.rng_cones) {
-            if !cone.is_symmetric() {
-                continue;
+        let mut innerfcn = |α: T, symcond: bool| -> T {
+            let mut α = α;
+            for (cone, rng) in zip(&mut self.cones, &self.rng_cones) {
+                if cone.is_symmetric() == symcond {
+                    continue;
+                }
+                let (dzi, dsi) = (&dz[rng.clone()], &ds[rng.clone()]);
+                let (zi, si) = (&z[rng.clone()], &s[rng.clone()]);
+                let (nextαz, nextαs) = cone.step_length(dzi, dsi, zi, si, settings, α);
+                α = T::min(α, T::min(nextαz, nextαs));
             }
-            let (dzi, dsi) = (&dz[rng.clone()], &ds[rng.clone()]);
-            let (zi, si) = (&z[rng.clone()], &s[rng.clone()]);
-            let (nextαz, nextαs) = cone.step_length(dzi, dsi, zi, si, settings, α);
-            α = T::min(α, T::min(nextαz, nextαs));
-        }
+            α
+        };
+
+        // Force symmetric cones first.
+        α = innerfcn(α, true);
 
         // if we have any nonsymmetric cones, then back off from full steps slightly
         // so that centrality checks and logarithms don't fail right at the boundaries
-
-        if !self.is_symmetric() {
+        if !all_symmetric {
             α = T::min(settings.max_step_fraction, α);
         }
+
         // Force asymmetric cones last.
-        for (cone, rng) in zip(&mut self.cones, &self.rng_cones) {
-            if cone.is_symmetric() {
-                continue;
-            }
-            let (dzi, dsi) = (&dz[rng.clone()], &ds[rng.clone()]);
-            let (zi, si) = (&z[rng.clone()], &s[rng.clone()]);
-            let (nextαz, nextαs) = cone.step_length(dzi, dsi, zi, si, settings, α);
-            α = T::min(α, T::min(nextαz, nextαs));
-        }
+        α = innerfcn(α, false);
 
         (α, α)
     }
 
     fn compute_barrier(&mut self, z: &[T], s: &[T], dz: &[T], ds: &[T], α: T) -> T {
         let mut barrier = T::zero();
         for (cone, rng) in zip(&mut self.cones, &self.rng_cones) {
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/expcone.rs` & `clarabel-0.8.0/src/solver/core/cones/expcone.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 
 // -------------------------------------
 // Exponential Cone
 // -------------------------------------
 
 pub struct ExponentialCone<T> {
     // Hessian of the dual barrier at z
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/genpowcone.rs` & `clarabel-0.8.0/src/solver/core/cones/genpowcone.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 use itertools::izip;
 use std::iter::zip;
 
 // -------------------------------------
 // Generalized Power Cone
 // -------------------------------------
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/mod.rs` & `clarabel-0.8.0/src/solver/core/cones/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/core/cones/nonnegativecone.rs` & `clarabel-0.8.0/src/solver/core/cones/nonnegativecone.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 use itertools::izip;
 use std::iter::zip;
 
 // -------------------------------------
 // Nonnegative Cone
 // -------------------------------------
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/nonsymmetric_common.rs` & `clarabel-0.8.0/src/solver/core/cones/nonsymmetric_common.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/core/cones/powcone.rs` & `clarabel-0.8.0/src/solver/core/cones/powcone.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 
 // -------------------------------------
 // Power Cone
 // -------------------------------------
 
 pub struct PowerCone<T> {
     // power defining the cone
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/psdtrianglecone.rs` & `clarabel-0.8.0/src/solver/core/cones/psdtrianglecone.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 
 // ------------------------------------
 // Positive Semidefinite Cone (Scaled triangular form)
 // ------------------------------------
 
 pub struct PSDConeData<T> {
     chol1: CholeskyEngine<T>,
     chol2: CholeskyEngine<T>,
     SVD: SVDEngine<T>,
     Eig: EigEngine<T>,
     λ: Vec<T>,
     Λisqrt: Vec<T>,
     R: Matrix<T>,
     Rinv: Matrix<T>,
-    kronRR: Matrix<T>,
-    B: Matrix<T>,
     Hs: Matrix<T>,
 
     //workspace for various internal uses
     workmat1: Matrix<T>,
     workmat2: Matrix<T>,
     workmat3: Matrix<T>,
     workvec: Vec<T>,
@@ -41,16 +36,14 @@
             SVD: SVDEngine::<T>::new((n, n)),
             Eig: EigEngine::<T>::new(n),
 
             λ: vec![T::zero(); n],
             Λisqrt: vec![T::zero(); n],
             R: Matrix::zeros((n, n)),
             Rinv: Matrix::zeros((n, n)),
-            kronRR: Matrix::zeros((n * n, n * n)),
-            B: Matrix::zeros((Bm, n * n)),
             Hs: Matrix::zeros((Bm, Bm)),
 
             //workspace for various internal uses
             workmat1: Matrix::zeros((n, n)),
             workmat2: Matrix::zeros((n, n)),
             workmat3: Matrix::zeros((n, n)),
             workvec: vec![T::zero(); triangular_number(n)],
@@ -113,15 +106,15 @@
         let β: T;
 
         if z.is_empty() {
             α = T::max_value();
             β = T::zero();
         } else {
             let Z = &mut self.data.workmat1;
-            _svec_to_mat(Z, z);
+            svec_to_mat(Z, z);
             self.data.Eig.eigvals(Z).expect("Eigval error");
             let e = &self.data.Eig.λ;
             α = e.minimum();
             β = e.iter().fold(T::zero(), |s, x| s + T::max(*x, T::zero())); //= sum(e[e.>0])
         }
 
         (α, β)
@@ -158,62 +151,58 @@
         if s.is_empty() {
             //bail early on zero length cone
             return true;
         }
 
         let f = &mut self.data;
         let (S, Z) = (&mut f.workmat1, &mut f.workmat2);
-        _svec_to_mat(S, s);
-        _svec_to_mat(Z, z);
+        svec_to_mat(S, s);
+        svec_to_mat(Z, z);
 
         //compute Cholesky factors
-        let c1 = f.chol1.cholesky(S);
-        let c2 = f.chol2.cholesky(Z);
+        let c1 = f.chol1.factor(S);
+        let c2 = f.chol2.factor(Z);
 
         // bail if the cholesky factorization fails
         // PJG: Need proper Result return type here
         if c1.is_err() || c2.is_err() {
             return false;
         }
 
         let (L1, L2) = (&f.chol1.L, &f.chol2.L);
 
         // SVD of L2'*L1,
         let tmp = &mut f.workmat1;
         tmp.mul(&L2.t(), L1, T::one(), T::zero());
-        f.SVD.svd(tmp).expect("SVD error");
+        f.SVD.factor(tmp).expect("SVD error");
 
         // assemble λ (diagonal), R and Rinv.
         f.λ.copy_from(&f.SVD.s);
         f.Λisqrt.copy_from(&f.λ).sqrt().recip();
 
         //f.R = L1*(f.SVD.V)*f.Λisqrt
         f.R.mul(L1, &f.SVD.Vt.t(), T::one(), T::zero());
         f.R.rscale(&f.Λisqrt);
 
         //f.Rinv .= f.Λisqrt*(f.SVD.U)'*L2'
         f.Rinv.mul(&f.SVD.U.t(), &L2.t(), T::one(), T::zero());
         f.Rinv.lscale(&f.Λisqrt);
 
-        // we should compute here the upper triangular part
-        // of the matrix Q* (RR^T) ⨂ (RR^T) * P.  The operator
-        // P is a matrix that transforms a packed triangle to
-        // a vectorized full matrix.
-
-        f.kronRR.kron(&f.R, &f.R);
-
-        // B .= Q'*kRR, where Q' is the svec operator
-        for i in 0..f.B.ncols() {
-            let M = ReshapedMatrix::from_slice(f.kronRR.col_slice(i), f.R.nrows(), f.R.nrows());
-            let b = f.B.col_slice_mut(i);
-            _mat_to_svec(b, &M);
-        }
-
-        // compute Hs = triu(B*B')
-        f.Hs.syrk(&f.B, T::one(), T::zero());
+        // compute R*R^T (upper triangular part only)
+        let RRt = &mut f.workmat1;
+        RRt.data_mut().set(T::zero());
+        RRt.syrk(&f.R, T::one(), T::zero());
+
+        // PJG: it is possibly faster to compute the whole of RRt, and not
+        // just the upper triangle using syrk!, because then skron! can be
+        // be called with a Matrix type instead of Symmetric.   The internal
+        // indexing within skron! is then more straightforward and probably
+        // faster.   Possibly also worth considering a version of skron!
+        // that uses unchecked indexing.
+        skron(&mut f.Hs, &RRt.sym());
 
         true //PJG: Should return result, with "?" operators above
     }
 
     fn Hs_is_diagonal(&self) -> bool {
         false
     }
@@ -253,42 +242,42 @@
         αmax: T,
     ) -> (T, T) {
         let Λisqrt = &self.data.Λisqrt;
         let d = &mut self.data.workvec;
         let engine = &mut self.data.Eig;
 
         // d = Δz̃ = WΔz
-        _mul_Wx_inner(
+        mul_Wx_inner(
             MatrixShape::N,
             d,
             dz,
             T::one(),
             T::zero(),
             &self.data.R,
             &mut self.data.workmat1,
             &mut self.data.workmat2,
             &mut self.data.workmat3,
         );
         let workΔ = &mut self.data.workmat1;
-        let αz = _step_length_psd_component(workΔ, engine, d, Λisqrt, αmax);
+        let αz = step_length_psd_component(workΔ, engine, d, Λisqrt, αmax);
 
         // d = Δs̃ = W^{-T}Δs
-        _mul_Wx_inner(
+        mul_Wx_inner(
             MatrixShape::T,
             d,
             ds,
             T::one(),
             T::zero(),
             &self.data.Rinv,
             &mut self.data.workmat1,
             &mut self.data.workmat2,
             &mut self.data.workmat3,
         );
         let workΔ = &mut self.data.workmat1;
-        let αs = _step_length_psd_component(workΔ, engine, d, Λisqrt, αmax);
+        let αs = step_length_psd_component(workΔ, engine, d, Λisqrt, αmax);
 
         (αz, αs)
     }
 
     fn compute_barrier(&mut self, z: &[T], s: &[T], dz: &[T], ds: &[T], α: T) -> T {
         let mut barrier = T::zero();
         barrier -= self.logdet_barrier(z, dz, α);
@@ -303,17 +292,17 @@
 {
     fn logdet_barrier(&mut self, x: &[T], dx: &[T], α: T) -> T
     where
         T: FloatT,
     {
         let (Q, q) = (&mut self.data.workmat1, &mut self.data.workvec);
         q.waxpby(T::one(), x, α, dx);
-        _svec_to_mat(Q, q);
+        svec_to_mat(Q, q);
 
-        match self.data.chol1.cholesky(Q) {
+        match self.data.chol1.factor(Q) {
             Ok(_) => self.data.chol1.logdet(),
             Err(_) => T::infinity(),
         }
     }
 }
 
 // ---------------------------------------------
@@ -325,73 +314,73 @@
     T: FloatT,
 {
     // implements x = λ \ z for the SDP cone
     fn λ_inv_circ_op(&mut self, x: &mut [T], z: &[T]) {
         let X = &mut self.data.workmat1;
         let Z = &mut self.data.workmat2;
 
-        _svec_to_mat(X, x);
-        _svec_to_mat(Z, z);
+        svec_to_mat(X, x);
+        svec_to_mat(Z, z);
 
         let λ = &self.data.λ;
         let two: T = (2.).as_T();
         for i in 0..self.n {
             for j in 0..self.n {
                 X[(i, j)] = (two * Z[(i, j)]) / (λ[i] + λ[j]);
             }
         }
-        _mat_to_svec(x, X);
+        mat_to_svec(x, X);
     }
 
     fn mul_W(&mut self, is_transpose: MatrixShape, y: &mut [T], x: &[T], α: T, β: T) {
-        _mul_Wx_inner(
+        mul_Wx_inner(
             is_transpose,
             y,
             x,
             α,
             β,
             &self.data.R,
             &mut self.data.workmat1,
             &mut self.data.workmat2,
             &mut self.data.workmat3,
         )
     }
 
     fn mul_Winv(&mut self, is_transpose: MatrixShape, y: &mut [T], x: &[T], α: T, β: T) {
-        _mul_Wx_inner(
+        mul_Wx_inner(
             is_transpose,
             y,
             x,
             α,
             β,
             &self.data.Rinv,
             &mut self.data.workmat1,
             &mut self.data.workmat2,
             &mut self.data.workmat3,
         )
     }
 }
 
 #[allow(clippy::too_many_arguments)]
-fn _mul_Wx_inner<T>(
+fn mul_Wx_inner<T>(
     is_transpose: MatrixShape,
     y: &mut [T],
     x: &[T],
     α: T,
     β: T,
     Rx: &Matrix<T>,
     workmat1: &mut Matrix<T>,
     workmat2: &mut Matrix<T>,
     workmat3: &mut Matrix<T>,
 ) where
     T: FloatT,
 {
     let (X, Y, tmp) = (workmat1, workmat2, workmat3);
-    _svec_to_mat(X, x);
-    _svec_to_mat(Y, y);
+    svec_to_mat(X, x);
+    svec_to_mat(Y, y);
 
     match is_transpose {
         MatrixShape::T => {
             // Y .= α*(R*X*R') + βY        #W^T*x,   or....
             // Y .= α*(Rinv*X*Rinv') + βY  #W^{-T}*x
             tmp.mul(X, &Rx.t(), T::one(), T::zero());
             Y.mul(Rx, tmp, α, β);
@@ -399,15 +388,15 @@
         MatrixShape::N => {
             // Y .= α*(R'*X*R) + βY         #W*x
             // Y .= α*(Rinv'*X*Rinv) + βY   #W^{-1}*x
             tmp.mul(&Rx.t(), X, T::one(), T::zero());
             Y.mul(tmp, Rx, α, β);
         }
     }
-    _mat_to_svec(y, Y);
+    mat_to_svec(y, Y);
 }
 
 // ---------------------------------------------
 // Jordan algebra operations for symmetric cones
 // ---------------------------------------------
 
 impl<T> JordanAlgebra<T> for PSDTriangleCone<T>
@@ -416,22 +405,22 @@
 {
     fn circ_op(&mut self, x: &mut [T], y: &[T], z: &[T]) {
         let (Y, Z, X) = (
             &mut self.data.workmat1,
             &mut self.data.workmat2,
             &mut self.data.workmat3,
         );
-        _svec_to_mat(Y, y);
-        _svec_to_mat(Z, z);
+        svec_to_mat(Y, y);
+        svec_to_mat(Z, z);
 
         // X .= (Y*Z + Z*Y)/2
         // NB: works b/c Y and Z are both symmetric
         X.data_mut().set(T::zero()); //X.sym() will assert is_triu
         X.syr2k(Y, Z, (0.5).as_T(), T::zero());
-        _mat_to_svec(x, &X.sym());
+        mat_to_svec(x, &X.sym());
     }
 
     fn inv_circ_op(&mut self, _x: &mut [T], _y: &[T], _z: &[T]) {
         // X should be the solution to (YX + XY)/2 = Z
 
         //  For general arguments this requires solution to a symmetric
         // Sylvester equation.  Throwing an error here since I do not think
@@ -441,103 +430,77 @@
     }
 }
 
 //-----------------------------------------
 // internal operations for SDP cones
 // ----------------------------------------
 
-fn _step_length_psd_component<T>(
+fn step_length_psd_component<T>(
     workΔ: &mut Matrix<T>,
     engine: &mut EigEngine<T>,
     d: &[T],
     Λisqrt: &[T],
     αmax: T,
 ) -> T
 where
     T: FloatT,
 {
     let γ = {
         if d.is_empty() {
             T::max_value()
         } else {
-            _svec_to_mat(workΔ, d);
+            svec_to_mat(workΔ, d);
             workΔ.lrscale(Λisqrt, Λisqrt);
             engine.eigvals(workΔ).expect("Eigval error");
             engine.λ.minimum()
         }
     };
 
     if γ < T::zero() {
         T::min(-γ.recip(), αmax)
     } else {
         αmax
     }
 }
 
-fn _svec_to_mat<T: FloatT>(M: &mut Matrix<T>, x: &[T]) {
-    let mut idx = 0;
-    for col in 0..M.ncols() {
-        for row in 0..=col {
-            if row == col {
-                M[(row, col)] = x[idx];
-            } else {
-                M[(row, col)] = x[idx] * T::FRAC_1_SQRT_2();
-                M[(col, row)] = x[idx] * T::FRAC_1_SQRT_2();
-            }
-            idx += 1;
-        }
-    }
-}
-
-//PJG : Perhaps implementation for Symmetric type would be faster
-fn _mat_to_svec<MAT, T: FloatT>(x: &mut [T], M: &MAT)
+// produce the upper triangular part of the Symmetric Kronecker product of
+// a symmtric matrix A with itself, i.e. triu(A ⊗_s A)
+fn skron<T>(out: &mut Matrix<T>, A: &Symmetric<Matrix<T>>)
 where
-    MAT: DenseMatrix<T = T, Output = T>,
+    T: FloatT,
 {
-    let mut idx = 0;
-    for col in 0..M.ncols() {
-        for row in 0..=col {
-            x[idx] = {
-                if row == col {
-                    M[(row, col)]
-                } else {
-                    (M[(row, col)] + M[(col, row)]) * T::FRAC_1_SQRT_2()
-                }
-            };
-            idx += 1;
-        }
-    }
-}
-
-#[test]
-
-fn test_svec_conversions() {
-    let n = 3;
-
-    let X = Matrix::from(&[
-        [1., 3., -2.], //
-        [3., -4., 7.], //
-        [-2., 7., 5.], //
-    ]);
-
-    let Y = Matrix::from(&[
-        [2., 5., -4.],  //
-        [5., 6., 2.],   //
-        [-4., 2., -3.], //
-    ]);
-
-    let mut Z = Matrix::zeros((3, 3));
-
-    let mut x = vec![0.; triangular_number(n)];
-    let mut y = vec![0.; triangular_number(n)];
-
-    // check inner product identity
-    _mat_to_svec(&mut x, &X);
-    _mat_to_svec(&mut y, &Y);
-
-    assert!(f64::abs(x.dot(&y) - X.data().dot(Y.data())) < 1e-12);
+    let sqrt2 = T::SQRT_2();
+    let n = A.nrows();
 
-    // check round trip
-    _mat_to_svec(&mut x, &X);
-    _svec_to_mat(&mut Z, &x);
-    assert!(X.data().norm_inf_diff(Z.data()) < 1e-12);
+    let mut col = 0;
+    for l in 0..n {
+        for k in 0..=l {
+            let mut row = 0;
+            let kl_eq = k == l;
+
+            for j in 0..n {
+                let Ajl = A[(j, l)];
+                let Ajk = A[(j, k)];
+
+                for i in 0..=j {
+                    if row > col {
+                        break;
+                    }
+
+                    let ij_eq = i == j;
+
+                    out[(row, col)] = {
+                        match (ij_eq, kl_eq) {
+                            (false, false) => A[(i, k)] * Ajl + A[(i, l)] * Ajk,
+                            (true, false) => sqrt2 * Ajl * Ajk,
+                            (false, true) => sqrt2 * A[(i, l)] * Ajk,
+                            (true, true) => Ajl * Ajl,
+                        }
+                    };
+
+                    row += 1;
+                } //end i
+            } //end j
+            col += 1;
+        } //end k
+    } //end l
 }
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/socone.rs` & `clarabel-0.8.0/src/solver/core/cones/socone.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 use itertools::izip;
 
 // -------------------------------------
 // Second order Cone
 // -------------------------------------
 
 pub struct SecondOrderConeSparseData<T> {
@@ -220,16 +217,14 @@
     }
 
     fn get_Hs(&self, Hsblock: &mut [T]) {
         if let Some(sparse_data) = &self.sparse_data {
             // For sparse form, we are returning here the diagonal D block
             // from the sparse representation of W^TW, but not the
             // extra two entries at the bottom right of the block.
-            // The ConicVector for s and z (and its views) don't
-            // know anything about the 2 extra sparsifying entries
             Hsblock.fill(self.η * self.η);
             Hsblock[0] *= sparse_data.d;
         } else {
             let two: T = (2.).as_T();
             // for dense form, we return H = \eta^2 (2*ww^T - J), where
             // J = diag(1,-I).  We are packing into dense triu form
             Hsblock[0] = two * self.w[0] * self.w[0] - T::one();
@@ -410,15 +405,15 @@
 // compute the residual at z + \alpha dz
 // without storing the intermediate vector
 fn _soc_residual_shifted<T>(z: &[T], dz: &[T], α: T) -> T
 where
     T: FloatT,
 {
     let x0 = z[0] + α * dz[0];
-    let x1_sq = <[T] as VectorMath>::dot_shifted(&z[1..], &z[1..], &dz[1..], &dz[1..], α);
+    let x1_sq = <[T] as VectorMath<T>>::dot_shifted(&z[1..], &z[1..], &dz[1..], &dz[1..], α);
 
     x0 * x0 - x1_sq
 }
 
 // find the maximum step length α≥0 so that
 // x + αy stays in the SOC
 fn _step_length_soc_component<T>(x: &[T], y: &[T], αmax: T) -> T
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/supportedcone.rs` & `clarabel-0.8.0/src/solver/core/cones/supportedcone.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use super::*;
-use crate::algebra::FloatT;
 
 #[cfg(feature = "sdp")]
 use crate::algebra::triangular_number;
 
 // ---------------------------------------------------
 // We define some machinery here for enumerating the
 // different cone types that can live in the composite cone
@@ -190,7 +189,68 @@
             SupportedConeTag::PowerCone => "PowerCone",
             #[cfg(feature = "sdp")]
             SupportedConeTag::PSDTriangleCone => "PSDTriangleCone",
             SupportedConeTag::GenPowerCone => "GenPowerCone",
         }
     }
 }
+
+// ----------------------------------------------
+// Iterator for the range of indices of the cone
+
+//PJG: type names are not satisfactory.   Try to combine
+//with the internal cone generators.
+
+#[cfg_attr(not(sdp), allow(dead_code))]
+pub(crate) struct RangeSupportedConesIterator<'a, T> {
+    cones: &'a [SupportedConeT<T>],
+    index: usize,
+    start: usize,
+}
+
+#[cfg_attr(not(sdp), allow(dead_code))]
+impl<'a, T> Iterator for RangeSupportedConesIterator<'a, T> {
+    type Item = std::ops::Range<usize>;
+
+    fn next(&mut self) -> Option<Self::Item> {
+        if self.index < self.cones.len() {
+            let cone = &self.cones[self.index];
+            let stop = self.start + cone.nvars();
+            let range = self.start..stop;
+            self.index += 1;
+            self.start = stop;
+            Some(range)
+        } else {
+            None
+        }
+    }
+}
+#[cfg_attr(not(sdp), allow(dead_code))]
+pub(crate) trait ConeRanges<'a, T> {
+    fn rng_cones_iter(&'a self) -> RangeSupportedConesIterator<'a, T>;
+}
+
+#[cfg_attr(not(sdp), allow(dead_code))]
+impl<'a, T> ConeRanges<'a, T> for [SupportedConeT<T>] {
+    fn rng_cones_iter(&'a self) -> RangeSupportedConesIterator<'a, T> {
+        RangeSupportedConesIterator::<'a, T> {
+            cones: self,
+            index: 0,
+            start: 0,
+        }
+    }
+}
+
+#[test]
+fn test_cone_ranges() {
+    let cones = [
+        SupportedConeT::NonnegativeConeT::<f64>(3),
+        SupportedConeT::NonnegativeConeT::<f64>(0),
+        SupportedConeT::SecondOrderConeT::<f64>(4),
+    ];
+
+    let rngs: Vec<std::ops::Range<usize>> = vec![0..3, 3..3, 3..7];
+
+    for (rng, conerng) in std::iter::zip(rngs.iter(), cones.rng_cones_iter()) {
+        assert_eq!(*rng, conerng);
+    }
+}
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/symmetric_common.rs` & `clarabel-0.8.0/src/solver/core/cones/symmetric_common.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::algebra::{FloatT, MatrixShape, VectorMath};
+use crate::algebra::{MatrixShape, VectorMath};
 
 use super::*;
 
 // --------------------------------------
 // Traits and blanket implementations for Exponential and PowerCones
 // -------------------------------------
 
@@ -11,19 +11,21 @@
     // Multiplication by the scaling point
     fn mul_W(&mut self, is_transpose: MatrixShape, y: &mut [T], x: &[T], α: T, β: T);
     fn mul_Winv(&mut self, is_transpose: MatrixShape, y: &mut [T], x: &[T], α: T, β: T);
 
     // x = λ \ z
     // Included as a special case since q \ z for general q is difficult
     // to implement for general q i PSD cone and never actually needed.
+    #[allow(dead_code)] //PJG: not currently used anywhere
     fn λ_inv_circ_op(&mut self, x: &mut [T], z: &[T]);
 }
 
 pub trait JordanAlgebra<T: FloatT> {
     fn circ_op(&mut self, x: &mut [T], y: &[T], z: &[T]);
+    #[allow(dead_code)] //PJG: inv_circ_op not needed anywhere.  keep for symmetry
     fn inv_circ_op(&mut self, x: &mut [T], y: &[T], z: &[T]);
 }
 
 // --------------------------------------
 // Trait with blanket implementation for all symmetric cones
 // Provides functions that are identical across types
```

### Comparing `clarabel-0.7.1/src/solver/core/cones/zerocone.rs` & `clarabel-0.8.0/src/solver/core/cones/zerocone.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 use super::*;
-use crate::{
-    algebra::*,
-    solver::{core::ScalingStrategy, CoreSettings},
-};
+use crate::algebra::*;
 use core::marker::PhantomData;
 
 // -------------------------------------
 // Zero Cone
 // -------------------------------------
 
 pub struct ZeroCone<T> {
```

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     fn solve(
         &mut self,
         lhsx: Option<&mut [T]>,
         lhsz: Option<&mut [T]>,
         settings: &CoreSettings<T>,
     ) -> bool {
-        self.ldlsolver.solve(&mut self.x, &self.b);
+        self.ldlsolver.solve(&self.KKT, &mut self.x, &self.b);
 
         let is_success = {
             if settings.iterative_refinement_enable {
                 self.iterative_refinement(settings)
             } else {
                 self.x.is_finite()
             }
@@ -270,15 +270,15 @@
                 //within tolerance.  Exit
                 break;
             }
 
             let lastnorme = norme;
 
             //make a refinement
-            self.ldlsolver.solve(dx, e);
+            self.ldlsolver.solve(K, dx, e);
 
             //prospective solution is x + dx.  Use dx space to
             // hold it for a check before applying to x
             dx.axpby(T::one(), x, T::one());
 
             norme = _get_refine_error(e, b, K, dx);
 
@@ -327,15 +327,15 @@
 fn _get_ldlsolver_config<T>(settings: &CoreSettings<T>) -> (MatrixTriangle, LDLConstructor<T>)
 where
     T: FloatT,
 {
     //The Julia version implements this using a module scope dictionary,
     //which allows users to register custom solver types.  That seems much
     //harder to do in Rust since a static mutable Hashmap is unsafe.  For
-    //now, we use a fixed lookup table, so any new suppored solver types
+    //now, we use a fixed lookup table, so any new supported solver types
     //supported must be added here.   It should be possible to allow a
     //"custom" LDL solver in the settings in well, whose constructor and
     //and matrix shape could then be registered as some (probably hidden)
     //options in the settings.
 
     let ldlptr: LDLConstructor<T>;
     let kktshape: MatrixTriangle;
```

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #![allow(non_snake_case)]
 
 use super::datamaps::*;
 use crate::algebra::*;
-use crate::solver::core::cones::CompositeCone;
 use crate::solver::core::cones::*;
 use num_traits::Zero;
 
 pub(crate) fn allocate_kkt_Hsblocks<T, Z>(cones: &CompositeCone<T>) -> Vec<Z>
 where
     T: FloatT,
     Z: Zero + Clone,
```

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.factors.scale_values(index, scale);
     }
 
     fn offset_values(&mut self, index: &[usize], offset: T, signs: &[i8]) {
         self.factors.offset_values(index, offset, signs);
     }
 
-    fn solve(&mut self, x: &mut [T], b: &[T]) {
+    fn solve(&mut self, _kkt: &CscMatrix<T>, x: &mut [T], b: &[T]) {
         // NB: QDLDL solves in place
         x.copy_from(b);
         self.factors.solve(x);
     }
 
     fn refactor(&mut self, _kkt: &CscMatrix<T>) -> bool {
         //QDLDL has maintained its own version of the permuted
```

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/direct/quasidef/mod.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/direct/quasidef/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 use datamaps::*;
 pub use directldlkktsolver::*;
 use kkt_assembly::*;
 
 pub trait DirectLDLSolver<T: FloatT> {
     fn update_values(&mut self, index: &[usize], values: &[T]);
     fn scale_values(&mut self, index: &[usize], scale: T);
+    #[allow(dead_code)] //PJG: could be removed.
     fn offset_values(&mut self, index: &[usize], offset: T, signs: &[i8]);
-    fn solve(&mut self, x: &mut [T], b: &[T]);
+    fn solve(&mut self, kkt: &CscMatrix<T>, x: &mut [T], b: &[T]);
     fn refactor(&mut self, kkt: &CscMatrix<T>) -> bool;
     fn required_matrix_shape() -> MatrixTriangle
     where
         Self: Sized;
 }
```

### Comparing `clarabel-0.7.1/src/solver/core/kktsolvers/mod.rs` & `clarabel-0.8.0/src/solver/core/kktsolvers/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/core/solver.rs` & `clarabel-0.8.0/src/solver/core/solver.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 // ---------------------------------
 // Solver status type
 // ---------------------------------
 
 /// Status of solver at termination
 
 #[repr(u32)]
-#[derive(PartialEq, Eq, Clone, Debug, Copy)]
+#[derive(PartialEq, Eq, Clone, Debug, Copy, Default)]
 pub enum SolverStatus {
     /// Problem is not solved (solver hasn't run).
+    #[default]
     Unsolved,
     /// Solver terminated with a solution.
     Solved,
     /// Problem is primal infeasible.  Solution returned is a certificate of primal infeasibility.
     PrimalInfeasible,
     /// Problem is dual infeasible.  Solution returned is a certificate of dual infeasibility.
     DualInfeasible,
@@ -85,20 +86,14 @@
 
 impl std::fmt::Display for SolverStatus {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         write!(f, "{:?}", self)
     }
 }
 
-impl Default for SolverStatus {
-    fn default() -> Self {
-        SolverStatus::Unsolved
-    }
-}
-
 // ---------------------------------
 // top level solver container type
 // ---------------------------------
 
 // The top-level solver.
 
 // This trait is defined with a collection of mutually interacting associated types.
@@ -128,17 +123,24 @@
 
     writeln!(
         out,
         "-------------------------------------------------------------"
     )?;
     writeln!(
         out,
-        "           Clarabel.rs v{}  -  Clever Acronym              \n",
+        "           Clarabel.rs v{}  -  Clever Acronym                ",
         crate::VERSION
     )?;
+    #[cfg(debug_assertions)]
+    writeln!(
+        out,
+        "                  *** debug build ***                        ",
+    )?;
+    #[cfg(not(debug_assertions))]
+    writeln!(out)?;
     writeln!(
         out,
         "                   (c) Paul Goulart                          "
     )?;
     writeln!(
         out,
         "                University of Oxford, 2022                   "
@@ -172,15 +174,15 @@
     T: FloatT,
     D: ProblemData<T, V = V>,
     V: Variables<T, D = D, R = R, C = C, SE = SE>,
     R: Residuals<T, D = D, V = V>,
     K: KKTSystem<T, D = D, V = V, C = C, SE = SE>,
     C: Cone<T>,
     I: Info<T, D = D, V = V, R = R, C = C, SE = SE>,
-    SO: Solution<T, D = D, V = V, I = I>,
+    SO: Solution<T, D = D, V = V, I = I, SE = SE>,
     SE: Settings<T>,
 {
     fn solve(&mut self) {
         // various initializations
         let mut iter: u32 = 0;
         let mut σ = T::one();
         let mut α = T::zero();
@@ -253,15 +255,18 @@
                         StrategyCheckpoint::Update(s) => {scaling = s; continue}
                     }
             }  // allows continuation if new strategy provided
 
 
             // update the scalings
             // --------------
-            let is_scaling_success = self.variables.scale_cones(&mut self.cones,μ,scaling);
+            let is_scaling_success;
+            timeit!{timers => "scale cones"; {
+                is_scaling_success = self.variables.scale_cones(&mut self.cones,μ,scaling);
+            }}
             // check whether variables are interior points
             match self.strategy_checkpoint_is_scaling_success(is_scaling_success,scaling){
                 StrategyCheckpoint::Fail => {break}
                 StrategyCheckpoint::NoUpdate => {} // we only expect NoUpdate or Fail here
                 StrategyCheckpoint::Update(_) => {unreachable!()}
             }
 
@@ -370,32 +375,35 @@
         // Check we if actually took a final step.  If not, we need
         // to recapture the scalars and print one last line
         if α == T::zero() {
             self.info.save_scalars(μ, α, σ, iter);
             notimeit! {timers; {self.info.print_status(&self.settings).unwrap();}}
         }
 
-        //store final solution, timing etc
-        self.info
-            .finalize(&self.residuals, &self.settings, &mut timers);
+        timeit! {timers => "post-process"; {
+            //check for "almost" convergence case and then extract solution
+            self.info.post_process(&self.residuals, &self.settings);
+            self.solution
+                .post_process(&self.data, &mut self.variables, &self.info, &self.settings);
+        }}
 
-        self.solution
-            .finalize(&self.data, &self.variables, &self.info);
+        //halt timers
+        self.info.finalize(&mut timers);
+        self.solution.finalize(&self.info);
 
         self.info.print_footer(&self.settings).unwrap();
 
         //stow the timers back into Option in the solver struct
         self.timers.replace(timers);
     }
 }
 
 // Encapsulate the internal helpers trait in a private module
 // so it doesn't get exported
 mod internal {
-    use super::super::cones::Cone;
     use super::super::traits::*;
     use super::*;
 
     pub(super) trait IPSolverInternals<T, D, V, R, K, C, I, SO, SE> {
         /// Find an initial condition
         fn default_start(&mut self);
```

### Comparing `clarabel-0.7.1/src/solver/core/traits.rs` & `clarabel-0.8.0/src/solver/core/traits.rs`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,19 @@
 {
     type V: Variables<T>;
     type R: Residuals<T>;
 
     /// Reset internal data, particularly solve timers.
     fn reset(&mut self, timers: &mut Timers);
 
+    /// Final convergence checks, e.g. for "almost" convergence cases
+    fn post_process(&mut self, residuals: &Self::R, settings: &Self::SE);
+
     /// Compute final values before solver termination
-    fn finalize(&mut self, residuals: &Self::R, settings: &Self::SE, timers: &mut Timers);
+    fn finalize(&mut self, timers: &mut Timers);
 
     /// Update solver progress information
     fn update(
         &mut self,
         data: &mut Self::D,
         variables: &Self::V,
         residuals: &Self::R,
@@ -214,17 +217,27 @@
 
 /// Solution for a conic optimization problem.
 
 pub trait Solution<T: FloatT> {
     type D: ProblemData<T>;
     type V: Variables<T>;
     type I: Info<T>;
+    type SE: Settings<T>;
 
     /// Compute solution from the Variables at solver termination
-    fn finalize(&mut self, data: &Self::D, variables: &Self::V, info: &Self::I);
+    fn post_process(
+        &mut self,
+        data: &Self::D,
+        variables: &mut Self::V,
+        info: &Self::I,
+        settings: &Self::SE,
+    );
+
+    /// finalize the solution, e.g. extract final timing from info
+    fn finalize(&mut self, info: &Self::I);
 }
 
 /// Settings for a conic optimization problem.
 ///
 /// Implementors of this trait can define any internal or problem
 /// specific settings they wish.   They must, however, also maintain
 /// a settings object of type [`CoreSettings`](crate::solver::core::CoreSettings)
```

### Comparing `clarabel-0.7.1/src/solver/implementations/default/data_updating.rs` & `clarabel-0.8.0/src/solver/implementations/default/data_updating.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/implementations/default/equilibration.rs` & `clarabel-0.8.0/src/solver/implementations/default/equilibration.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/implementations/default/info.rs` & `clarabel-0.8.0/src/solver/implementations/default/info.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,30 +55,28 @@
         self.status = SolverStatus::Unsolved;
         self.iterations = 0;
         self.solve_time = 0f64;
 
         timers.reset_timer("solve");
     }
 
-    fn finalize(
-        &mut self,
-        residuals: &DefaultResiduals<T>,
-        settings: &DefaultSettings<T>,
-        timers: &mut Timers,
-    ) {
+    fn post_process(&mut self, residuals: &DefaultResiduals<T>, settings: &DefaultSettings<T>) {
         // if there was an error or we ran out of time
         // or iterations, check for partial convergence
 
         if self.status.is_errored()
             || matches!(self.status, SolverStatus::MaxIterations)
             || matches!(self.status, SolverStatus::MaxTime)
         {
             self.check_convergence_almost(residuals, settings);
         }
+    }
 
+    fn finalize(&mut self, timers: &mut Timers) {
+        //final check of timers
         self.solve_time = timers.total_time().as_secs_f64();
     }
 
     fn update(
         &mut self,
         data: &mut DefaultProblemData<T>,
         variables: &DefaultVariables<T>,
```

### Comparing `clarabel-0.7.1/src/solver/implementations/default/info_print.rs` & `clarabel-0.8.0/src/solver/implementations/default/info_print.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#[cfg(feature = "sdp")]
+use crate::solver::chordal::ChordalInfo;
+
 use crate::stdio;
 use crate::{
     algebra::*,
     solver::core::cones::{SupportedConeAsTag, SupportedConeTag},
 };
 use std::io::Write;
 
@@ -33,26 +36,32 @@
     fn print_configuration(
         &self,
         settings: &DefaultSettings<T>,
         data: &DefaultProblemData<T>,
         cones: &CompositeCone<T>,
     ) -> std::io::Result<()> {
         if !settings.verbose {
-            return std::io::Result::Ok(())
+            return std::io::Result::Ok(());
         }
 
         let mut out = stdio::stdout();
 
-        if data.presolver.is_reduced() {
-            writeln!(out, 
+        if let Some(ref presolver) = data.presolver {
+            writeln!(
+                out,
                 "\npresolve: removed {} constraints",
-                data.presolver.count_reduced()
+                presolver.count_reduced()
             )?;
         }
 
+        #[cfg(feature = "sdp")]
+        if let Some(ref chordal_info) = data.chordal_info {
+            print_chordal_decomposition(chordal_info, settings)?;
+        }
+
         writeln!(out, "\nproblem:")?;
         writeln!(out, "  variables     = {}", data.n)?;
         writeln!(out, "  constraints   = {}", data.m)?;
         writeln!(out, "  nnz(P)        = {}", data.P.nnz())?;
         writeln!(out, "  nnz(A)        = {}", data.A.nnz())?;
         writeln!(out, "  cones (total) = {}", cones.len())?;
 
@@ -62,40 +71,40 @@
         _print_conedims_by_type(cones, SupportedConeTag::SecondOrderCone)?;
         _print_conedims_by_type(cones, SupportedConeTag::ExponentialCone)?;
         _print_conedims_by_type(cones, SupportedConeTag::PowerCone)?;
         _print_conedims_by_type(cones, SupportedConeTag::GenPowerCone)?;
         #[cfg(feature = "sdp")]
         _print_conedims_by_type(cones, SupportedConeTag::PSDTriangleCone)?;
 
-        writeln!(out, )?;
+        writeln!(out,)?;
         _print_settings(settings)?;
-        writeln!(out, )?;
+        writeln!(out,)?;
 
         std::io::Result::Ok(())
     }
 
     fn print_status_header(&self, settings: &DefaultSettings<T>) -> std::io::Result<()> {
         if !settings.verbose {
-            return std::io::Result::Ok(())
+            return std::io::Result::Ok(());
         }
 
         let mut out = stdio::stdout();
 
         //print a subheader for the iterations info
         write!(out, "iter    ")?;
         write!(out, "pcost        ")?;
         write!(out, "dcost       ")?;
         write!(out, "gap       ")?;
         write!(out, "pres      ")?;
         write!(out, "dres      ")?;
         write!(out, "k/t       ")?;
         write!(out, " μ       ")?;
         write!(out, "step      ")?;
-        writeln!(out, )?;
-        writeln!(out, 
+        writeln!(out,)?;
+        writeln!(out,
             "---------------------------------------------------------------------------------------------"
         )?;
         stdio::stdout().flush()?;
         std::io::Result::Ok(())
     }
 
     fn print_status(&self, settings: &DefaultSettings<T>) -> std::io::Result<()> {
@@ -117,33 +126,34 @@
 
         if self.iterations > 0 {
             write!(out, "{}  ", expformat!("{:>.2e}", self.step_length))?;
         } else {
             write!(out, " ------   ")?; //info.step_length
         }
 
-        writeln!(out, )?;
+        writeln!(out,)?;
 
         std::io::Result::Ok(())
     }
 
     fn print_footer(&self, settings: &DefaultSettings<T>) -> std::io::Result<()> {
         if !settings.verbose {
             return std::io::Result::Ok(());
         }
 
         let mut out = stdio::stdout();
 
-        writeln!(out, 
+        writeln!(out,
             "---------------------------------------------------------------------------------------------"
         )?;
 
         writeln!(out, "Terminated with status = {}", self.status)?;
 
-        writeln!(out, 
+        writeln!(
+            out,
             "solve time = {:?}",
             Duration::from_secs_f64(self.solve_time)
         )?;
 
         std::io::Result::Ok(())
     }
 }
@@ -151,95 +161,158 @@
 fn _bool_on_off(v: bool) -> &'static str {
     match v {
         true => "on",
         false => "false",
     }
 }
 
-fn _print_settings<T: FloatT>(settings: &DefaultSettings<T>) -> std::io::Result<()>{
+fn _print_settings<T: FloatT>(settings: &DefaultSettings<T>) -> std::io::Result<()> {
     let set = settings;
     let mut out = stdio::stdout();
 
     writeln!(out, "settings:")?;
 
     if set.direct_kkt_solver {
-        writeln!(out, 
+        writeln!(
+            out,
             "  linear algebra: direct / {}, precision: {} bit",
             set.direct_solve_method,
             _get_precision_string::<T>()
         )?;
     }
 
     let time_lim_str = {
         if set.time_limit.is_infinite() {
             "Inf".to_string()
         } else {
             format!("{:?}", set.time_limit)
         }
     };
-    writeln!(out, 
+    writeln!(
+        out,
         "  max iter = {}, time limit = {},  max step = {:.3}",
         set.max_iter, time_lim_str, set.max_step_fraction
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "  tol_feas = {:.1e}, tol_gap_abs = {:.1e}, tol_gap_rel = {:.1e},",
         set.tol_feas, set.tol_gap_abs, set.tol_gap_rel
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "  static reg : {}, ϵ1 = {:.1e}, ϵ2 = {:.1e}",
         _bool_on_off(set.static_regularization_enable),
         set.static_regularization_constant,
         set.static_regularization_proportional,
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "  dynamic reg: {}, ϵ = {:.1e}, δ = {:.1e}",
         _bool_on_off(set.dynamic_regularization_enable),
         set.dynamic_regularization_eps,
         set.dynamic_regularization_delta
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "  iter refine: {}, reltol = {:.1e}, abstol = {:.1e},",
         _bool_on_off(set.iterative_refinement_enable),
         set.iterative_refinement_reltol,
         set.iterative_refinement_abstol
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "               max iter = {}, stop ratio = {:.1}",
         set.iterative_refinement_max_iter, set.iterative_refinement_stop_ratio
     )?;
 
-    writeln!(out, 
+    writeln!(
+        out,
         "  equilibrate: {}, min_scale = {:.1e}, max_scale = {:.1e}",
         _bool_on_off(set.equilibrate_enable),
         set.equilibrate_min_scaling,
         set.equilibrate_max_scaling
     )?;
 
-    writeln!(out, "               max iter = {}", set.equilibrate_max_iter,)?;
+    writeln!(
+        out,
+        "               max iter = {}",
+        set.equilibrate_max_iter,
+    )?;
+
+    std::io::Result::Ok(())
+}
+
+#[cfg(feature = "sdp")]
+fn print_chordal_decomposition<T: FloatT>(
+    chordal_info: &ChordalInfo<T>,
+    settings: &DefaultSettings<T>,
+) -> std::io::Result<()> {
+    let mut out = stdio::stdout();
+
+    writeln!(out, "\nchordal decomposition:")?;
+    writeln!(
+        out,
+        "  compact format = {}, dual completion = {}",
+        _bool_on_off(settings.chordal_decomposition_compact),
+        _bool_on_off(settings.chordal_decomposition_complete_dual)
+    )?;
+
+    writeln!(
+        out,
+        "  merge method = {}",
+        settings.chordal_decomposition_merge_method
+    )?;
+
+    writeln!(
+        out,
+        "  PSD cones initial             = {}",
+        chordal_info.init_psd_cone_count()
+    )?;
+
+    writeln!(
+        out,
+        "  PSD cones decomposable        = {}",
+        chordal_info.decomposable_cone_count()
+    )?;
+
+    writeln!(
+        out,
+        "  PSD cones after decomposition = {}",
+        chordal_info.premerge_psd_cone_count()
+    )?;
+
+    writeln!(
+        out,
+        "  PSD cones after merges        = {}",
+        chordal_info.final_psd_cone_count()
+    )?;
 
     std::io::Result::Ok(())
 }
 
 fn _get_precision_string<T: FloatT>() -> String {
     (::std::mem::size_of::<T>() * 8).to_string()
 }
 
-fn _print_conedims_by_type<T: FloatT>(cones: &CompositeCone<T>, conetag: SupportedConeTag) -> std::io::Result<()> {
+fn _print_conedims_by_type<T: FloatT>(
+    cones: &CompositeCone<T>,
+    conetag: SupportedConeTag,
+) -> std::io::Result<()> {
     let maxlistlen = 5;
 
     let count = cones.get_type_count(conetag);
 
     //skip if there are none of this type
     if count == 0 {
-        return std::io::Result::Ok(())
+        return std::io::Result::Ok(());
     }
 
     let mut out = stdio::stdout();
 
     // how many of this type of cone?
     let name = conetag.as_str();
 
@@ -269,15 +342,15 @@
         write!(out, " numel = (")?;
         for nvar in nvars.iter().take(maxlistlen - 1) {
             write!(out, "{},", nvar)?;
         }
         write!(out, "...,{})", nvars[nvars.len() - 1])?;
     }
 
-    writeln!(out, )?;
+    writeln!(out,)?;
 
     std::io::Result::Ok(())
 }
 
 // convert a string in LowerExp display format into one that
 // 1) always has a sign after the exponent, and
 // 2) has at least two digits in the exponent.
```

### Comparing `clarabel-0.7.1/src/solver/implementations/default/kktsystem.rs` & `clarabel-0.8.0/src/solver/implementations/default/kktsystem.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/implementations/default/mod.rs` & `clarabel-0.8.0/src/solver/implementations/default/mod.rs`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 mod solver;
 mod variables;
 
 // export flattened
 pub use data_updating::*;
 pub use equilibration::*;
 pub use info::*;
-pub use info_print::*;
 pub use kktsystem::*;
 pub use presolver::*;
 pub use problemdata::*;
 pub use residuals::*;
 pub use settings::*;
 pub use solution::*;
 pub use solver::*;
```

### Comparing `clarabel-0.7.1/src/solver/implementations/default/presolver.rs` & `clarabel-0.8.0/src/solver/chordal/decomp/psd_completion.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,133 @@
-#![allow(non_snake_case)]
-use super::*;
 use crate::algebra::*;
-use crate::solver::SupportedConeT;
+use crate::solver::chordal::ChordalInfo;
+use crate::solver::chordal::SparsityPattern;
+use crate::solver::core::cones::*;
+use crate::solver::DefaultVariables;
+
+// -----------------------------------
+// psd completion
+// -----------------------------------
+
+// The psd entries of z that correspond to the zeros in s are not constrained by the problem.
+// however, in order to make the dual psd cone positive semidefinite we have to do a
+// positive semidefinite completion routine to choose the values
 
-// ---------------
-// Data type for default problem presolver
-// ---------------
-
-#[derive(Debug)]
-pub(crate) struct PresolverRowReductionIndex {
-    // vector of length = original RHS.   Entries are false
-    // for those rows that should be eliminated before solve
-    pub keep_logical: Vec<bool>,
-
-    // vector of length = reduced RHS, taking values
-    // that map reduced b back to their original index
-    // This is just findall(keep_logical) and is held for
-    // efficient solution repopulation
-    pub keep_index: Vec<usize>,
-}
-
-/// Presolver data for the standard solver implementation
-
-#[derive(Debug)]
-pub struct Presolver<T> {
-    // possibly reduced internal copy of user cone specification
-    pub(crate) cone_specs: Vec<SupportedConeT<T>>,
-
-    //record of reduced constraints for NN cones with inf bounds
-    pub(crate) reduce_map: Option<PresolverRowReductionIndex>,
-
-    // size of original and reduced RHS, respectively
-    pub(crate) mfull: usize,
-    pub(crate) mreduced: usize,
-
-    // inf bound that was taken from the module level
-    // and should be applied throughout.   Held here so
-    // that any subsequent change to the module's state
-    // won't mess up our solver mid-solve
-    pub(crate) infbound: f64,
-}
-
-impl<T> Presolver<T>
+impl<T> ChordalInfo<T>
 where
     T: FloatT,
 {
-    pub fn new(
-        _A: &CscMatrix<T>,
-        b: &[T],
-        cone_specs: &[SupportedConeT<T>],
-        settings: &DefaultSettings<T>,
-    ) -> Self {
-        let infbound = crate::solver::get_infinity();
-
-        // make copy of cone_specs to protect from user interference
-        let mut cone_specs = cone_specs.to_vec();
-        let mfull = b.len();
-
-        let (reduce_map, mreduced) = {
-            if settings.presolve_enable {
-                reduce_cones(&mut cone_specs, b, infbound.as_T())
-            } else {
-                (None, mfull)
-            }
-        };
-
-        Self {
-            cone_specs,
-            reduce_map,
-            mfull,
-            mreduced,
-            infbound,
+    pub(crate) fn psd_completion(&self, variables: &mut DefaultVariables<T>) {
+        // working now with the cones from the original
+        // problem, not the decomposed ones
+        let cones = &self.init_cones;
+
+        // loop over psd cones
+        let row_ranges: Vec<_> = cones.rng_cones_iter().collect();
+
+        // loop over just the patterns
+        for pattern in self.spatterns.iter() {
+            let row_range = row_ranges[pattern.orig_index].clone();
+            let z = &mut variables.z[row_range];
+            complete(z, pattern);
         }
     }
+}
 
-    pub fn is_reduced(&self) -> bool {
-        self.reduce_map.is_some()
-    }
-    pub fn count_reduced(&self) -> usize {
-        self.mfull - self.mreduced
-    }
+fn complete<T>(z: &mut [T], pattern: &SparsityPattern)
+where
+    T: FloatT,
+{
+    let n = pattern.ordering.len();
+    let mut Z = Matrix::zeros((n, n));
+    svec_to_mat(&mut Z, z);
+    psd_complete(&mut Z, pattern);
+    mat_to_svec(z, &Z);
 }
 
-fn reduce_cones<T>(
-    cone_specs: &mut [SupportedConeT<T>],
-    b: &[T],
-    infbound: T,
-) -> (Option<PresolverRowReductionIndex>, usize)
+// positive semidefinite completion (from Vandenberghe - Chordal Graphs..., p. 362)
+// input: A - positive definite completable matrix
+
+fn psd_complete<T>(A: &mut Matrix<T>, pattern: &SparsityPattern)
 where
     T: FloatT,
 {
-    //assume we keep everything initially
-    let mut keep_logical = vec![true; b.len()];
-    let mut mreduced = b.len();
-
-    // we loop through b and remove any entries that are both infinite
-    // and in a nonnegative cone
-
-    let mut is_reduced = false;
-    let mut bptr = 0; // index into the b vector
-
-    for cone in cone_specs.iter_mut() {
-        let numel_cone = cone.nvars();
-
-        // only try to reduce nn cones.  Make a slight contraction
-        // so that we are firmly "less than" here
-        let infbound = (T::one() - T::epsilon() * (10.).as_T()) * infbound;
-
-        if matches!(cone, SupportedConeT::NonnegativeConeT(_)) {
-            let mut num_finite = 0;
-            for i in bptr..(bptr + numel_cone) {
-                if b[i] < infbound {
-                    num_finite += 1;
-                } else {
-                    keep_logical[i] = false;
-                    mreduced -= 1;
-                }
+    let sntree = &pattern.sntree;
+    let p = &pattern.ordering;
+    let ip = invperm(p);
+    let N = A.ncols();
+
+    // PJG: not clear to me if this copy of A is required, or
+    // whether I can operate directly on A by permuting the
+    // the indices in the loops below.  Only worth doing that
+    // if copying in or out of A is expensive.
+
+    // permutate matrix based on ordering p
+    // W is in the order that the cliques are based on
+    let mut W = Matrix::zeros((N, N));
+    W.subsref(A, p, p);
+
+    // go through supernode tree in descending order (given a post-ordering).
+    // This is ensured in the get_snode, get_separators functions
+
+    let mut Wαα = Matrix::<T>::zeros((0, 0));
+    let mut Wαν = Matrix::<T>::zeros((0, 0));
+    let mut Wηα = Matrix::<T>::zeros((0, 0));
+    let mut Wηα_times_Y = Matrix::<T>::zeros((0, 0));
+
+    let mut chol = CholeskyEngine::new(0);
+    let mut svd = SVDEngine::new((0, 0));
+
+    for j in (0..(sntree.n_cliques - 1)).rev() {
+        // in order to obtain ν, α the vertex numbers of the supernode are
+        // mapped to the new position of the permuted matrix index
+        // set of snd(i) sorted using the numerical ordering i,i+1,...i+ni
+        let ν = sntree.get_snode(j);
+
+        // index set containing the elements of col(i) \ snd(i)
+        // sorted using numerical ordering σ(i)
+        let α = sntree.get_separators(j);
+
+        // index set containing the row indices of the lower-triangular zeros in
+        // column i (i: representative index) sorted by σ(i)
+        let i = ν[0];
+        let η: Vec<usize> = ((i + 1)..N)
+            .filter(|&x| !α.contains(&x) && !ν.contains(&x))
+            .collect();
+
+        Wαα.resize((α.len(), α.len()));
+        Wαν.resize((α.len(), ν.len()));
+        Wηα.resize((η.len(), α.len()));
+
+        Wαα.subsref(&W, α, α);
+        Wαν.subsref(&W, α, ν);
+        Wηα.subsref(&W, &η, α);
+
+        // Solve WWαα \ Wαν.   First try Cholesky,
+        // and then fall back to pinv if it fails.
+        // NB: cholesky does not modify the matrix
+        // it factors, but the SVD call will
+        chol.resize(α.len());
+        match chol.factor(&mut Wαα) {
+            Ok(()) => {
+                chol.solve(&mut Wαν);
             }
-            if num_finite < numel_cone {
-                // contract the cone to a smaller size
-                *cone = SupportedConeT::NonnegativeConeT(num_finite);
-                is_reduced = true;
+            Err(_) => {
+                svd.resize((α.len(), α.len()));
+                svd.factor(&mut Wαα).unwrap();
+                svd.solve(&mut Wαν); //pinv solve
             }
         }
 
-        bptr += numel_cone;
-    }
+        let Y = &Wαν; //solved in place
+        Wηα_times_Y.resize((η.len(), ν.len()));
+        Wηα_times_Y.mul(&Wηα, Y, T::one(), T::zero());
 
-    let outoption = {
-        if is_reduced {
-            let keep_index = findall(&keep_logical);
-            Some(PresolverRowReductionIndex {
-                keep_logical,
-                keep_index,
-            })
-        } else {
-            None
-        }
-    };
+        W.subsasgn(&η, ν, &Wηα_times_Y);
 
-    (outoption, mreduced)
-}
+        // symmetry condition
+        W.subsasgn(ν, &η, &Wηα_times_Y.t());
+    }
 
-fn findall(keep_logical: &[bool]) -> Vec<usize> {
-    let map = keep_logical
-        .iter()
-        .enumerate()
-        .filter(|(_, &r)| r)
-        .map(|(index, _)| index)
-        .collect::<Vec<_>>();
-    map
+    // invert the permutation
+    A.subsref(&W, &ip, &ip);
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clarabel-0.7.1/src/solver/implementations/default/residuals.rs` & `clarabel-0.8.0/src/solver/implementations/default/residuals.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/implementations/default/solver.rs` & `clarabel-0.8.0/src/solver/implementations/default/solver.rs`

 * *Files 7% similar despite different names*

```diff
@@ -26,34 +26,38 @@
     T: FloatT,
 {
     pub fn new(
         P: &CscMatrix<T>,
         q: &[T],
         A: &CscMatrix<T>,
         b: &[T],
-        cone_specs: &[SupportedConeT<T>],
+        cones: &[SupportedConeT<T>],
         settings: DefaultSettings<T>,
     ) -> Self {
         //sanity check problem dimensions
-        _check_dimensions(P, q, A, b, cone_specs);
+        _check_dimensions(P, q, A, b, cones);
 
         let mut timers = Timers::default();
         let mut output;
         let info = DefaultInfo::<T>::new();
 
         timeit! {timers => "setup"; {
 
-        // reduce the cone sizes.  (A,b) will be reduced
-        // within the problem data constructor.  Also makes
-        // an internal copy of the user cone specification
-        let presolver = Presolver::<T>::new(A,b,cone_specs,&settings);
+        // user facing results go here.
+        let solution = DefaultSolution::<T>::new(A.n, A.m);
 
-        let cones = CompositeCone::<T>::new(&presolver.cone_specs);
-        let mut data = DefaultProblemData::<T>::new(P,q,A,b,presolver);
+        // presolve / chordal decomposition if needed,
+        // then take an internal copy of the problem data
+        let mut data;
+        timeit!{timers => "presolve"; {
+            data = DefaultProblemData::<T>::new(P,q,A,b,cones,&settings);
+        }}
 
+        let cones = CompositeCone::<T>::new(&data.cones);
+        assert_eq!(cones.numel, data.m);
         let variables = DefaultVariables::<T>::new(data.n,data.m);
         let residuals = DefaultResiduals::<T>::new(data.n,data.m);
 
         // equilibrate problem data immediately on setup.
         // this prevents multiple equlibrations if solve!
         // is called more than once.
         timeit!{timers => "equilibration"; {
@@ -66,17 +70,14 @@
         }}
 
         // work variables for assembling step direction LHS/RHS
         let step_rhs  = DefaultVariables::<T>::new(data.n,data.m);
         let step_lhs  = DefaultVariables::<T>::new(data.n,data.m);
         let prev_vars = DefaultVariables::<T>::new(data.n,data.m);
 
-        // user facing results go here.
-        let solution = DefaultSolution::<T>::new(data.presolver.mfull,data.n);
-
         output = Self{data,variables,residuals,kktsystem,step_lhs,
              step_rhs,prev_vars,info,solution,cones,settings,timers: None};
 
         }} //end "setup" timer.
 
         //now that the timer is finished we can swap our
         //timer object into the solver structure
```

### Comparing `clarabel-0.7.1/src/solver/mod.rs` & `clarabel-0.8.0/src/solver/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 pub(crate) const _INFINITY_DEFAULT: f64 = 1e20;
 // internal module structure
 pub(crate) mod core;
 pub mod implementations;
 pub(crate) mod utils;
 
+// chordal decomposition only if SDPs are enabled
+#[cfg(feature = "sdp")]
+pub(crate) mod chordal;
+
 //Here we expose only part of the solver internals
 //and rearrange public modules a bit to give a more
 //user friendly API
 
 pub use crate::solver::utils::infbounds::*;
 
 //allows declaration of cone constraints
@@ -30,15 +34,15 @@
 //user facing traits required to interact with solver
 pub use crate::solver::core::{IPSolver, SolverStatus};
 
 //user facing traits required to define new implementatiions
 pub use crate::solver::core::traits;
 pub use crate::solver::core::CoreSettings;
 
-//If we have implemtations for multple alternative
+//If we had implementations for multple alternative
 //problem formats, they would live here.   Since we
 //only have default, it is exposed at the top level
 //in the use statements directly below instead.
 
 // pub mod implementations {
 //     pub mod default {
 //         pub use clarabel_solver::implementations::default::*;
```

### Comparing `clarabel-0.7.1/src/solver/tests/cones.rs` & `clarabel-0.8.0/src/solver/tests/cones.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/utils/atomic.rs` & `clarabel-0.8.0/src/solver/utils/atomic.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/solver/utils/infbounds.rs` & `clarabel-0.8.0/src/solver/utils/infbounds.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/src/timers/timers.rs` & `clarabel-0.8.0/src/timers/timers.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/api_dimension_checks.rs` & `clarabel-0.8.0/tests/api_dimension_checks.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_eq_constrained.rs` & `clarabel-0.8.0/tests/basic_eq_constrained.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_expcone.rs` & `clarabel-0.8.0/tests/basic_expcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_genpowcone.rs` & `clarabel-0.8.0/tests/basic_genpowcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_lp.rs` & `clarabel-0.8.0/tests/basic_lp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_powcone.rs` & `clarabel-0.8.0/tests/basic_powcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_qp.rs` & `clarabel-0.8.0/tests/basic_qp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_sdp.rs` & `clarabel-0.8.0/tests/basic_sdp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_socp.rs` & `clarabel-0.8.0/tests/basic_socp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/basic_unconstrained.rs` & `clarabel-0.8.0/tests/basic_unconstrained.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/data_updating.rs` & `clarabel-0.8.0/tests/data_updating.rs`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 fn test_update_A_matrix_form() {
     // original problem
     let (P, q, A, b, cones, settings) = updating_test_data();
     let mut solver1 = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
     //solver1.solve();
 
     // change A and re-solve
-    let mut A2 = A.clone();
+    let mut A2 = A;
     A2.nzval[2] = -1000.;
 
     // intention was to update the entry at position (1,1).  Did it work?
     assert!(A2.get_entry((1, 1)).unwrap() == -1000.);
 
     // revised original solver
     assert!(solver1.update_A(&A2).is_ok());
@@ -138,15 +138,15 @@
 fn test_update_A_vector_form() {
     // original problem
     let (P, q, A, b, cones, settings) = updating_test_data();
     let mut solver1 = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
     solver1.solve();
 
     // change A and re-solve
-    let mut A2 = A.clone();
+    let mut A2 = A;
     A2.nzval[2] = -1000.;
 
     // intention was to update the entry at position (1,1).  Did it work?
     assert!(A2.get_entry((1, 1)).unwrap() == -1000.);
 
     // revised original solver
     assert!(solver1.update_A(&A2.nzval).is_ok());
@@ -170,15 +170,15 @@
     let values = [0.5, -0.5];
     let index = [1, 2];
     let Adata = zip(&index, &values);
     assert!(solver1.update_A(&Adata).is_ok());
     solver1.solve();
 
     //new solver
-    let mut A2 = A.clone();
+    let mut A2 = A;
     A2.nzval[1] = 0.5;
     A2.nzval[2] = -0.5;
     let mut solver2 = DefaultSolver::new(&P, &q, &A2, &b, &cones, settings);
     solver2.solve();
 
     assert!(solver1.solution.x.dist(&solver2.solution.x) <= 1e-7);
 }
@@ -187,15 +187,15 @@
 fn test_update_q() {
     // original problem
     let (P, q, A, b, cones, settings) = updating_test_data();
     let mut solver1 = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
     solver1.solve();
 
     // change 1 and re-solve
-    let mut q2 = q.clone();
+    let mut q2 = q;
     q2[1] = 10.;
 
     // revised original solver
     assert!(solver1.update_q(&q2).is_ok());
     solver1.solve();
 
     //new solver
@@ -216,15 +216,15 @@
     let values = [10.];
     let index = [1];
     let qdata = zip(&index, &values);
     assert!(solver1.update_q(&qdata).is_ok());
     solver1.solve();
 
     //new solver
-    let mut q2 = q.clone();
+    let mut q2 = q;
     q2[1] = 10.;
     let mut solver2 = DefaultSolver::new(&P, &q2, &A, &b, &cones, settings);
     solver2.solve();
 
     assert!(solver1.solution.x.dist(&solver2.solution.x) <= 1e-7);
 }
 
@@ -232,15 +232,15 @@
 fn test_update_b() {
     // original problem
     let (P, q, A, b, cones, settings) = updating_test_data();
     let mut solver1 = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
     solver1.solve();
 
     // change 1 and re-solve
-    let mut b2 = b.clone();
+    let mut b2 = b;
     b2[0] = 0.;
 
     // revised original solver
     assert!(solver1.update_b(&b2).is_ok());
     solver1.solve();
 
     //new solver
@@ -272,29 +272,29 @@
     assert!(solver1.solution.x.dist(&solver2.solution.x) <= 1e-7);
 }
 
 #[test]
 fn test_update_noops() {
     // original problem
     let (P, q, A, b, cones, settings) = updating_test_data();
-    let mut solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
+    let mut solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
     solver.solve();
 
     // apply no-op updates to check for crashes
     solver.update_P(&[]).unwrap();
     solver.update_A(&[]).unwrap();
     solver.update_q(&[]).unwrap();
     solver.update_b(&[]).unwrap();
 
     // try noops in various combinations
-    let P2 = P.clone().to_triu();
-    let A2 = A.clone();
-    let b2 = b.clone();
+    let P2 = P.to_triu();
+    let A2 = A;
+    let b2 = b;
     let b2zip = zip(&[1, 3], &[0., 0.]);
-    let q2 = q.clone();
+    let q2 = q;
 
     solver.update_data(&[], &[], &[], &[]).unwrap();
     solver.update_data(&P2, &[], &A2, &[]).unwrap();
     solver.update_data(&P2.nzval, &[], &A2.nzval, &[]).unwrap();
     solver.update_data(&P2, &[], &A2.nzval, &[]).unwrap(); //mixed formats
     solver.update_data(&[], &q2, &[], &b2zip).unwrap(); //mixed formats
     solver.update_data(&P2.nzval, &[], &A2, &b2zip).unwrap(); //mixed formats
@@ -304,15 +304,15 @@
 }
 
 #[test]
 fn test_fail_on_presolve_enable() {
     // original problem
     let (P, q, A, b, cones, mut settings) = updating_test_data();
     settings.presolve_enable = true;
-    let mut solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings.clone());
+    let mut solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
     solver.solve();
 
     // apply no-op updates to check that updates are rejected
     assert!(matches!(
         solver.update_P(&[]).err(),
         Some(DataUpdateError::PresolveEnabled)
     ));
```

### Comparing `clarabel-0.7.1/tests/equilibration_bounds.rs` & `clarabel-0.8.0/tests/equilibration_bounds.rs`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 #[test]
 fn test_equilibrate_zero_rows() {
     let (P, c, mut A, b, cones) = equilibration_test_data();
     let settings = DefaultSettings::default();
 
     A.nzval.set(0.0);
 
-    let mut solver = DefaultSolver::new(&P, &c, &A, &b, &cones, settings.clone());
+    let mut solver = DefaultSolver::new(&P, &c, &A, &b, &cones, settings);
 
     solver.solve();
 
     let e = &solver.data.equilibration.e;
 
     assert!(e.iter().all(|&v| v == 1.));
 }
```

### Comparing `clarabel-0.7.1/tests/mixed_conic.rs` & `clarabel-0.8.0/tests/mixed_conic.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/tests/presolve.rs` & `clarabel-0.8.0/tests/presolve.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.7.1/PKG-INFO` & `clarabel-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: clarabel
-Version: 0.7.1
+Version: 0.8.0
 Classifier: Programming Language :: Rust
 Requires-Dist: numpy
 Requires-Dist: scipy
 License-File: LICENSE.md
 Summary: Clarabel Conic Interior Point Solver for Rust / Python
 Keywords: convex,optimization,conic,solver,linear-programming
 Author: Paul Goulart <paul.goulart@eng.ox.ac.uk>
@@ -22,24 +22,24 @@
 </picture>
 <h1 align="center" margin=0px>
 Interior Point Conic Optimization for Rust and Python
 </h1>
 <p align="center">
    <a href="https://github.com/oxfordcontrol/Clarabel.rs/actions"><img src="https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/oxfordcontrol/Clarabel.rs"><img src="https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/main/graph/badge.svg"></a>
-  <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
+  <a href="https://clarabel.org"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.7.1-blue.svg"></a>
+  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.8.0-blue.svg"></a>
 </p>
 
 <p align="center">
   <a href="#features">Features</a> •
   <a href="#installation">Installation</a> •
   <a href="#license-">License</a> •
-  <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable">Documentation</a>
+  <a href="https://clarabel.org">Documentation</a>
 </p>
 
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver for convex optimization problems using a novel homogeneous embedding.  Clarabel.rs solves the following problem:
 
 $$
 \begin{array}{r}
 \text{minimize} & \frac{1}{2}x^T P x + q^T x\\\\[2ex]
@@ -54,15 +54,15 @@
 and data matrices
 $P=P^\top \succeq 0$,
 $q \in \mathbb{R}^n$,
 $A \in \mathbb{R}^{m \times n}$, and
 $b \in \mathbb{R}^m$.
 The convex set $\mathcal{K}$ is a composition of convex cones.
 
-__For more information see the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/ClarabelDocs/stable) |  [dev](https://oxfordcontrol.github.io/ClarabelDocs/dev)).__
+__For more information see the Clarabel Documentation ([stable](https://clarabel.org) |  [dev](https://clarabel.org/dev)).__
 
 Clarabel is also available in a Julia implementation.  See [here](https://github.com/oxfordcontrol/Clarabel.jl).
  
 
 ## Features
 
 * __Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves problems with exponential, power cone and generalized power cone constraints.
```

#### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: clarabel Version: 0.7.1 Classifier: Programming
+Metadata-Version: 2.3 Name: clarabel Version: 0.8.0 Classifier: Programming
 Language :: Rust Requires-Dist: numpy Requires-Dist: scipy License-File:
 LICENSE.md Summary: Clarabel Conic Interior Point Solver for Rust / Python
 Keywords: convex,optimization,conic,solver,linear-programming Author: Paul
 Goulart
 eng.ox.ac.uk> Author-email: Paul Goulart
 eng.ox.ac.uk> License: Apache-2.0 Requires-Python: >=3.7 Description-Content-
 Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Source Code,
 https://github.com/oxfordcontrol/Clarabel.rs
                               [Clarabel.jl logo]
       ************ IInntteerriioorr PPooiinntt CCoonniicc OOppttiimmiizzaattiioonn ffoorr RRuusstt aanndd PPyytthhoonn ************
           _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_w_o_r_k_f_l_o_w_s_/_c_i_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_b_r_a_n_c_h_/
    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_s_t_a_b_l_e_-
 _p_u_r_p_l_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/
-                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._7_._1_-_b_l_u_e_._s_v_g_]
+                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._8_._0_-_b_l_u_e_._s_v_g_]
             _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _L_i_c_e_n_s_e â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver
 for convex optimization problems using a novel homogeneous embedding.
 Clarabel.rs solves the following problem: $$ \begin{array}{r} \text{minimize} &
 \frac{1}{2}x^T P x + q^T x\\\\[2ex] \text{subject to} & Ax + s = b \\\\[1ex] &
 s \in \mathcal{K} \end{array} $$ with decision variables $x \in \mathbb{R}^n$,
 $s \in \mathbb{R}^m$ and data matrices $P=P^\top \succeq 0$, $q \in \mathbb
 {R}^n$, $A \in \mathbb{R}^{m \times n}$, and $b \in \mathbb{R}^m$. The convex
 set $\mathcal{K}$ is a composition of convex cones. __For more information see
-the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/
-ClarabelDocs/stable) | [dev](https://oxfordcontrol.github.io/ClarabelDocs/
-dev)).__ Clarabel is also available in a Julia implementation. See [here]
-(https://github.com/oxfordcontrol/Clarabel.jl). ## Features * __Versatile__:
-Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-
-order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves
-problems with exponential, power cone and generalized power cone constraints. *
-__Quadratic objectives__: Unlike interior point solvers based on the standard
-homogeneous self-dual embedding (HSDE), Clarabel.rs handles quadratic
-objectives without requiring any epigraphical reformulation of the objective.
-It can therefore be significantly faster than other HSDE-based solvers for
-problems with quadratic objective functions. * __Infeasibility detection__:
-Infeasible problems are detected using a homogeneous embedding technique. *
-__Open Source__: Our code is available on [GitHub](https://github.com/
-oxfordcontrol/Clarabel.rs) and distributed under the Apache 2.0 License #
-Installation Clarabel can be imported to Cargo based Rust projects by adding
-```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml` file.
-To install from source, see the [Rust Installation Documentation](https://
-oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
+the Clarabel Documentation ([stable](https://clarabel.org) | [dev](https://
+clarabel.org/dev)).__ Clarabel is also available in a Julia implementation. See
+[here](https://github.com/oxfordcontrol/Clarabel.jl). ## Features *
+__Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs
+(QPs), second-order cone programs (SOCPs) and semidefinite programs (SDPs). It
+also solves problems with exponential, power cone and generalized power cone
+constraints. * __Quadratic objectives__: Unlike interior point solvers based on
+the standard homogeneous self-dual embedding (HSDE), Clarabel.rs handles
+quadratic objectives without requiring any epigraphical reformulation of the
+objective. It can therefore be significantly faster than other HSDE-based
+solvers for problems with quadratic objective functions. * __Infeasibility
+detection__: Infeasible problems are detected using a homogeneous embedding
+technique. * __Open Source__: Our code is available on [GitHub](https://
+github.com/oxfordcontrol/Clarabel.rs) and distributed under the Apache 2.0
+License # Installation Clarabel can be imported to Cargo based Rust projects by
+adding ```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml`
+file. To install from source, see the [Rust Installation Documentation](https:/
+/oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
 Python interface to the solver: ``` pip install clarabel ``` To install the
 Python interface from source, see the [Python Installation Documentation]
 (https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
 ## License ð This project is licensed under the Apache License 2.0 - see the
 [LICENSE.md](LICENSE.md) file for details.
```

