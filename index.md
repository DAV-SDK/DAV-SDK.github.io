---
layout: default
---

# DAV-SDK
{:.no_toc}

The data, analysis, and visualization (DAV) software development kit (SDK), or DAV-SDK, is an integration effort for the collection of data I/O & compression, analysis, and visualization software developed under the Department of Energy (DOE) Advanced Scientific Computing Research (ASCR). The software products target using [Spack](https://spack.io), an HPC-targeted source-based package manager, for deployment on HPC platforms and beyond. The primary product of this project is the [`dav-sdk`][spack_package] Spack meta-package which builds a set of DAV-SDK member packages together in a way that enables optimal features for target environments as well as interoperable features provided by other packages within the DAV-SDK. The DAV-SDK is an outcome of the work within the DOE PESO and OASIS projects.

[doe_ecp]: https://www.exascaleproject.org/
[spack_package]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/ecp-data-vis-sdk/package.py

* TOC bullet point is replaced by kramdown to generate table of contents.
{:toc}

## Included Projects

The following projects are included as part of the DAV SDK:

<span style="border-width:3px; border-style:solid; border-color:#fc8d59; padding: 0.5em;">[I/O](./io.html)</span>&emsp;
<span style="border-width:3px; border-style:solid; border-color:#ffffbf; padding: 0.5em;">[Compression](./compression.html)</span>&emsp;
<span style="border-width:3px; border-style:solid; border-color:#91bfdb; padding: 0.5em;">[Analysis and Visualization](./analysis-visualization.html)</span>

## Integration Status

<span style="border-width:3px; border-style:solid; border-color:#d73027; padding: 0.5em;">[General Spack](./general-spack.html)</span>&emsp;
<span style="border-width:3px; border-style:solid; border-color:#fc8d59; padding: 0.5em;">[DAV SDK](./dav-sdk.html)</span>&emsp;
<span style="border-width:3px; border-style:solid; border-color:#fee090; padding: 0.5em;">[E4S](./e4s.html)</span>

### Frontier

One of the primary challenges on Frontier is handling the compiler wrappers
for the CCE and AMD compilers, in particular how they wrap MPI and HIP.

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th>GCC Toolchain</th>
      <th>CCE Toolchain</th>
      <th>AMD Toolchain</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td>v11.2</td>  <!-- GCC Toolchain -->
      <td>v15.0.0</td>  <!-- CCE Toolchain -->
      <td>v5.3.0</td>  <!-- AMD Toolchain -->
    </tr>
    <tr>
      <td>
        Cray MPICH
      </td>  <!-- Info -->
      <td>v8.1.23</td>  <!-- GCC Toolchain -->
      <td>v8.1.23</td>  <!-- CCE Toolchain -->
      <td>v8.1.23</td>  <!-- AMD Toolchain -->
    </tr>
    <tr>
      <td>
        ROCm
      </td>  <!-- Info -->
      <td>v5.3.0</td>  <!-- GCC Toolchain -->
      <td>v5.3.0</td>  <!-- CCE Toolchain -->
      <td>v5.3.0</td>  <!-- AMD Toolchain -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th>GCC</th>
      <th>GCC + ROCm</th>
      <th>CCE</th>
      <th>CCE + ROCm</th>
      <th>AMD</th>
      <th>AMD + ROCm</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na" markdown="span">([1](#adios2_rocm))</td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na" markdown="span">([1](#adios2_rocm))</td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na" markdown="span">([1](#adios2_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="in_progress" markdown="span">([23](#unifyfs_frontier))</td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="in_progress" markdown="span">([23](#unifyfs_frontier))</td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na" markdown="span">([14](#veloc_rocm))</td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="in_progress" markdown="span">([3](#ascent_rocm))</td><!-- GCC + ROCm -->
      <td class="in_progress" markdown="span">([21](#ascent_find_mpi_frontier))</td><!-- CCE -->
      <td class="in_progress" markdown="span">([3](#ascent_rocm))</td><!-- CCE + ROCm -->
      <td class="in_progress" markdown="span">([21](#ascent_find_mpi_frontier))</td><!-- AMD -->
      <td class="in_progress" markdown="span">([3](#ascent_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="in_progress" markdown="span">([25](#cinema_frontier_python))</td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="verified"></td><!-- GCC + ROCm -->
      <td class="verified" markdown="span">([8](#paraview_no_ospray))</td><!-- CCE -->
      <td class="verified" markdown="span">([8](#paraview_no_ospray))</td><!-- CCE + ROCm -->
      <td class="verified" markdown="span">([8](#paraview_no_ospray))</td><!-- AMD -->
      <td class="verified" markdown="span">([8](#paraview_no_ospray))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- GCC -->
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- GCC + ROCm -->
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- CCE -->
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- CCE + ROCm -->
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- AMD -->
      <td class="in_progress" markdown="span">([12](#sensei_catalyst_backend))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na" markdown="span">([16](#visit_vtkm_support))</td><!-- GCC + ROCm -->
      <td class="in_progress"></td><!-- CCE -->
      <td class="na" markdown="span">([16](#visit_vtkm_support))</td><!-- CCE + ROCm -->
      <td class="in_progress"></td><!-- AMD -->
      <td class="na" markdown="span">([16](#visit_vtkm_support))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="verified" markdown="span">([18](#vtkm_rocm_openmp))</td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="verified" markdown="span">([18](#vtkm_rocm_openmp)) ([19](#vtkm_cray_wrapper_workaround))</td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="verified" markdown="span">([18](#vtkm_rocm_openmp)) ([19](#vtkm_cray_wrapper_workaround))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na"></td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na"></td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na" markdown="span">([20](#zfp_rocm))</td><!-- GCC + ROCm -->
      <td class="verified"></td><!-- CCE -->
      <td class="na" markdown="span">([20](#zfp_rocm))</td><!-- CCE + ROCm -->
      <td class="verified"></td><!-- AMD -->
      <td class="na" markdown="span">([20](#zfp_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td style="background-color: #373737; color: white">Legend</td>
      <td colspan="6">
        <table class="status_table_legend">
          <tr>
            <th class="verified" style="color: white;">Verified</th>
            <th class="in_progress" style="color: white;">In Progress</th>
            <th class="na" style="color: white;">Not Applicable</th>
            <th class="failing" style="color: white;">Failing</th>
          </tr>
        </table>
      </td>
    </tr>
  </tbody>
</table>

### Perlmutter Toolchains (CUDA)

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th>GCC Toolchain</th>
      <th>NVHPC Toolchain</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td>v11.2</td>  <!-- GCC Toolchain -->
      <td>v22.4</td>  <!-- NVHPC Toolchain -->
    </tr>
    <tr>
      <td>
        Cray MPICH
      </td>  <!-- Info -->
      <td>v8.2.3</td>  <!-- GCC Toolchain -->
      <td>v8.2.3</td>  <!-- NVHPC Toolchain -->
    </tr>
    <tr>
      <td>
        CUDA
      </td>  <!-- Info -->
      <td>v11.3</td>  <!-- GCC Toolchain -->
      <td>v11.3</td>  <!-- NVHPC Toolchain -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th>GCC</th>
      <th>GCC + CUDA</th>
      <th>NVHPC + CUDA</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na" markdown="span">([13](#veloc_cuda))</td><!-- GCC + CUDA -->
      <td class="na" markdown="span">([13](#veloc_cuda))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="failing" markdown="span">([2](#ascent_cuda_raja))</td><!-- GCC + CUDA -->
      <td class="na" markdown="span">([2](#ascent_cuda_raja))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na" markdown="span"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="na"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="in_progress"></td><!-- GCC -->
      <td class="na" markdown="span">([16](#visit_vtkm_support))</td><!-- GCC + CUDA -->
      <td class="na" markdown="span">([16](#visit_vtkm_support))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="verified" markdown="span"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [cuSZ][cuSZ]
      </td>
      <td class="na"></td><!-- GCC -->
      <td class="na"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified"></td><!-- GCC -->
      <td class="verified"></td><!-- GCC + CUDA -->
      <td class="na"></td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td style="background-color: #373737; color: white">Legend</td>
      <td colspan="3">
        <table class="status_table_legend">
          <tr>
            <th class="verified" style="color: white;">Verified</th>
            <th class="in_progress" style="color: white;">In Progress</th>
            <th class="na" style="color: white;">Not Applicable</th>
            <th class="failing" style="color: white;">Failing</th>
          </tr>
        </table>
      </td>
    </tr>
  </tbody>
</table>


### Aurora/Sunspot Toolchains

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th>GCC</th>
      <th>OneAPI</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td>v11.2.0</td>  <!-- GCC Toolchain -->
      <td>v2023.0.0</td>  <!-- OneAPI Toolchain -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th>GCC</th>
      <th>OneAPI</th>
      <th markdown="span">SYCL ([*](#oneapi_sycl))</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="in_progress" markdown="span">([5](#cinema_oneapi_python))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="in_progress"></td><!-- GCC -->
      <td class="in_progress" markdown="span">([8](#paraview_no_ospray)) ([9](#paraview_oneapi_python))</td><!-- OneApi -->
      <td class="in_progress" markdown="span">([7](#paraview_oneapi_sycl))</td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="in_progress"></td><!-- GCC -->
      <td class="in_progress" markdown="span">([10](#sensei_ospray)) ([12](#sensei_catalyst_backend))</td><!-- OneApi -->
      <td class="in_progress" markdown="span">([11](#sensei_kokkos)) ([12](#sensei_catalyst_backend))</td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="in_progress"></td><!-- GCC -->
      <td class="in_progress"></td><!-- OneApi -->
      <td class="in_progress" markdown="span">([16](#visit_vtkm_support))</td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="in_progress"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" markdown="span">([**](#verified_on_sunspot))</td><!-- OneApi -->
      <td class="na"></td><!-- OneApi -->
    </tr>
    <tr>
      <td style="background-color: #373737; color: white">Legend</td>
      <td colspan="3">
        <table class="status_table_legend">
          <tr>
            <th class="verified" style="color: white;">Verified</th>
            <th class="in_progress" style="color: white;">In Progress</th>
            <th class="na" style="color: white;">Not Applicable</th>
            <th class="failing" style="color: white;">Failing</th>
          </tr>
        </table>
      </td>
    </tr>
  </tbody>
</table>

## Notes

<!-- NOTE: we want to group the notes and link to them from the table, so we
     will be creating anchor "span"s with id attributes to href to above. -->

<span id="oneapi_sycl">**SYCL**</span> - SYCL extensions are implemented and tested using OneAPI.

<span id="verified_on_sunspot">\*\* </span> Due to the similarity between the toolchains on Aurora and Sunspot, the results for the Aurora system are currently marked as verified as builds on Aurora progress. As issues are found on Aurora, these values will be updated to reflect the target system status.

<span id="adios2_rocm">**ADIOS2**</span> - ROCm/HIP support is not expected in near term release.

<span id="ascent_cuda_raja">**Ascent**</span> - Blocked by build errors in RAJA package.

<span id="ascent_rocm">**Ascent**</span> - The spack recipe does not have support for ROCm. It is in under development in the Alpine Spack fork.

<span id="ascent_no_sycl">**Ascent**</span> - Ascent currently does not have any known plans for explicit SYCL support.

<span id="ascent_perlmutter_mpi">**Ascent**</span> - The way MPI is set up on Perlmutter conflicts with Ascent's spack recipe and CMake. Fixes for this are being developed.

<span id="ascent_find_mpi_frontier">**Ascent**</span> - Using the CCE toolchain has issues locating MPI with CMake.

<span id="cinema_oneapi_python">**Cinema**</span> - Failure to build a number of Python modules with OneAPI.

<span id="cinema_frontier_python">**Cinema**</span> - Failure to build working python modules for some of Cinemas dependency modules.

<span id="darshan_runtime_hdf5">**Darshan**</span> - Darshan with HDF5 integration enabled does not support use cases that do not link HDF5 in the same runtime environment.

<span id="paraview_oneapi_sycl">**ParaView**</span> - ParaView and VisIt do not support building SYCL kernels for VTK-m filters in released versions.

<span id="paraview_no_ospray">**ParaView**</span> - OSPRay support has been disabled due to build errors.

<span id="paraview_oneapi_python">**ParaView**</span> - Failure to build a number of Python modules with OneAPI.

<span id="sensei_ospray">**SENSEI**</span> - SENSEI is developing native OSPRay rendering support.

<span id="sensei_kokkos">**SENSEI**</span> - SENSEI is developing Kokkos support for ROCm, CUDA, and SYCL interop.

<span id="sensei_catalyst_backend">**SENSEI**</span> - SENSEI is developing updates to support ParaView v5.11 and Catalyst 2.

<span id="unifyfs_frontier">**UnifyFS**</span> - UnifyFS has a link error when using the Cray wrappers for the Cray and AMD toolchains.

<span id="veloc_cuda">**VeloC**</span> - CUDA support for VeloC is under development.

<span id="veloc_rocm">**VeloC**</span> - Kokkos/ROCm support for VeloC is experimental in [kokkos-resilience](https://github.com/kokkos/kokkos-resilience)

<span id="visit_hdf5_conflict">**VisIt**</span> - VisIt utilizes a VTK version locked to a Python that is not compatible with the Python requirements of PyH5, the HDF5 python interface used by Cinema.

<span id="visit_vtkm_support">**VisIt**</span> - VTK-m enabled GPU support is available VisIt, but is not officially tested as part of the Data and Vis SDK due to ([15](#visit_hdf5_conflict)) only recently being resolved.

<span id="vtkm_rocm_openmp">**VTK-m**</span> - Spack ROCm does not provide OpenMP correclty for VTKm HIP modules.

<span id="vtkm_cray_wrapper_workaround">**VTK-m**</span> - Frontier requires additional workarounds in the Spack recipe for VTKm that are specific to the Cray wrappers on Frontier. [patch](https://github.com/spack/spack/pull/34427)

<span id="zfp_rocm">**ZFP**</span> - ROCm support is under development.


[ADIOS2]: https://csmd.ornl.gov/software/adios2
[Darshan]: https://www.mcs.anl.gov/research/projects/darshan/
[HDF5]: https://www.hdfgroup.org/solutions/hdf5/
[PNetCDF]: https://parallel-netcdf.github.io/
[UnifyFS]: https://unifyfs.readthedocs.io/en/latest/
[VeloC]: https://veloc.readthedocs.io/en/latest/
[Ascent]: https://github.com/Alpine-DAV/ascent
[Cinema]: https://cinemascience.github.io
[ParaView]: https://paraview.org
[SENSEI]: https://sensei-insitu.org/
[VisIt]: https://visit-dav.github.io/visit-website/
[VTK-m]: https://m.vtk.org
[SZ]: https://szcompressor.org
[cuSZ]: https://github.com/szcompressor/cuSZ
[ZFP]: https://computing.llnl.gov/projects/zfp