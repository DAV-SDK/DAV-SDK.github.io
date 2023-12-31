---
layout: default
---

## Frontier Support

[back](./)

## Toolchains

One of the primary challenges on Frontier is handling the compiler wrappers
for the CCE and AMD compilers, in particular how they wrap MPI and HIP.

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th style="text-align: center">GCC</th>
      <th style="text-align: center">CCE</th>
      <th style="text-align: center">AMD</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td style="text-align: center">v11.2</td>  <!-- GCC -->
      <td style="text-align: center">v15.0.0</td>  <!-- CCE -->
      <td style="text-align: center">v5.3.0</td>  <!-- AMD -->
    </tr>
    <tr>
      <td>
        Cray MPICH
      </td>  <!-- Info -->
      <td style="text-align: center">v8.1.23</td>  <!-- GCC -->
      <td style="text-align: center">v8.1.23</td>  <!-- CCE -->
      <td style="text-align: center">v8.1.23</td>  <!-- AMD -->
    </tr>
    <tr>
      <td>
        ROCm
      </td>  <!-- Info -->
      <td style="text-align: center">v5.3.0</td>  <!-- GCC -->
      <td style="text-align: center">v5.3.0</td>  <!-- CCE -->
      <td style="text-align: center">v5.3.0</td>  <!-- AMD -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th style="text-align: center">GCC</th>
      <th style="text-align: center">GCC + ROCm</th>
      <th style="text-align: center">CCE</th>
      <th style="text-align: center">CCE + ROCm</th>
      <th style="text-align: center">AMD</th>
      <th style="text-align: center">AMD + ROCm</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#adios2_rocm))</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#adios2_rocm))</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#adios2_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#unifyfs_frontier))</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#unifyfs_frontier))</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#veloc_rocm))</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#veloc_rocm))</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#veloc_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_rocm))</td><!-- GCC + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_find_mpi_frontier))</td><!-- CCE -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_rocm))</td><!-- CCE + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_find_mpi_frontier))</td><!-- AMD -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_rocm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#cinema_frontier_python))</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="verified" style="text-align: center">✅</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#paraview_no_ospray))</td><!-- CCE -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#paraview_no_ospray))</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#paraview_no_ospray))</td><!-- AMD -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#paraview_no_ospray))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- GCC + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- CCE -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- CCE + ROCm -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- AMD -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#visit_vtkm))</td><!-- GCC + ROCm -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- CCE -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#visit_vtkm))</td><!-- CCE + ROCm -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- AMD -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#visit_vtkm))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#vtkm_rocm_openmp))</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">🔎</td><!-- CCE -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#vtkm_rocm_openmp) [✅](#vtkm_cray_wrapper_workaround))</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">🔎</td><!-- AMD -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#vtkm_rocm_openmp) [✅](#vtkm_cray_wrapper_workaround))</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [cuSZ][cuSZ]
      </td>
      <td class="na" style="text-align: center">N/A</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE -->
      <td class="na" style="text-align: center">N/A</td><!-- CCE + ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD -->
      <td class="na" style="text-align: center">N/A</td><!-- AMD + ROCm -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#zfp_rocm))</td><!-- GCC + ROCm -->
      <td class="verified" style="text-align: center">🔎</td><!-- CCE -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#zfp_rocm))</td><!-- CCE + ROCm -->
      <td class="verified" style="text-align: center">🔎</td><!-- AMD -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#zfp_rocm))</td><!-- AMD + ROCm -->
    </tr>
  </tbody>
</table>

<p style="text-align:center; border-width:3px; border-style:solid; border-color:#4393c3; padding: 0.5em;">✅ - <b>Verified</b>&emsp;🔎 - <b>In Progress</b>&emsp;🚫 - <b>Broken</b>&emsp;N/A - <b>Not Applicable</b></p>

[back](./)

## Notes

<span id="oneapi_sycl">**SYCL**</span> - [SYCL](https://www.khronos.org/sycl/) extensions are implemented and tested using [oneAPI](https://www.intel.com/content/www/us/en/developer/tools/oneapi/overview.html).

<span id="adios2_rocm">**ADIOS2**</span> - ADIOS2 ROCm/HIP support is not expected in near term release.

<span id="unifyfs_frontier">**UnifyFS**</span> - UnifyFS has a link error when using the Cray wrappers for the Cray and AMD toolchains.

<span id="ascent_find_mpi_frontier">**Ascent**</span> - Using the CCE toolchain has issues locating MPI with CMake.

<span id="ascent_rocm">**Ascent**</span> - Ascent spack recipe does not have support for ROCm. It is in under development in the Alpine Spack fork.

<span id="cinema_frontier_python">**Cinema**</span> - Failure to build working python modules for some of Cinemas dependency modules.

<span id="paraview_no_ospray">**ParaView**</span> - OSPRay support has been disabled due to build errors.

<span id="sensei_catalyst">**SENSEI**</span> - SENSEI is developing updates to support ParaView v5.11 and Catalyst 2.

<span id="visit_hdf5_conflict">**VisIt**</span> - VisIt utilizes a VTK version locked to a Python that is not compatible with the Python requirements of PyH5, the HDF5 python interface used by Cinema.

<span id="visit_vtkm">**VisIt**</span> - VTK-m enabled GPU support for CUDA and ROCm is available VisIt, but is not officially tested as part of the DAV-SDK due to ([HDF5 conflict](#visit_hdf5_conflict)) only recently being resolved.

<span id="vtkm_rocm_openmp">**VTK-m**</span> - Spack ROCm does not provide OpenMP correclty for VTKm HIP modules.

<span id="vtkm_cray_wrapper_workaround">**VTK-m**</span> - Frontier requires additional workarounds in the Spack recipe for VTKm that are specific to the Cray wrappers on Frontier. [patch](https://github.com/spack/spack/pull/34427)

<span id="veloc_rocm">**VeloC**</span> - VeloC ROCm (Kokkos) support for VeloC is experimental in [kokkos-resilience](https://github.com/kokkos/kokkos-resilience)

<span id="zfp_rocm">**ZFP**</span> - ZFP ROCm support is under development.

[back](./)

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
