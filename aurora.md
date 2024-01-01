---
layout: default
---

## Perlmutter Support

[back](./)

## Toolchains

The primary challenges on Aurora is handling the compiler wrapper
for the oneAPI compilers, in particular how they wrap MPI and SYCL.

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th style="text-align: center">GCC</th>
      <th style="text-align: center">oneAPI</th>
      <th style="text-align: center">SYCL</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td style="text-align: center">v11.2.0</td>  <!-- GCC  -->
      <td style="text-align: center">v2023.0.0</td>  <!-- oneAPI -->
      <td style="text-align: center">v???</td>  <!-- oneAPI -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th style="text-align: center">GCC</th>
      <th style="text-align: center">oneAPI</th>
      <th style="text-align: center" markdown="span">oneAPI + ([SYCL](#verified_on_sunspot))</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#hdf5_vol-daos))</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#cinema_oneapi_python))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="in_progress" style="text-align: center">🔎</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#paraview_no_ospray) [🔎](#paraview_no_ospray))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#paraview_oneapi_sycl))</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_ospray) [🔎](#sensei_catalyst))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_kokkos) [🔎](#sensei_catalyst))</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="in_progress" style="text-align: center">🔎</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#visit_vtkm) [🔎](#paraview_no_ospray))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#vtkm-sycl))</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [cuSZ][cuSZ]
      </td>
      <td class="na" style="text-align: center">N/A</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI -->
      <td class="na" style="text-align: center">N/A</td><!-- oneAPI + SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- GCC -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#verified_on_sunspot))</td><!-- oneAPI -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#zfp-sycl))</td><!-- oneAPI + SYCL -->
    </tr>
  </tbody>
</table>

<p style="text-align:center; border-width:3px; border-style:solid; border-color:#4393c3; padding: 0.5em;">✅ - <b>Verified</b>&emsp;🔎 - <b>In Progress</b>&emsp;🚫 - <b>Broken</b>&emsp;N/A - <b>Not Applicable</b></p>

[back](./)

## Notes

<span id="verified_on_sunspot">**Aurora**</span> - Due to the similarity between the toolchains on Aurora and Sunspot, the results for the Aurora system are currently marked as verified as builds on Aurora progress. As issues are found on Aurora, these values will be updated to reflect the target system status.

<span id="cinema_oneapi_python">**Cinema**</span> - Failure to build a number of Python modules with OneAPI.

<span id="hdf5_vol-daos">**HDF5**</span> - HDF5 vol DAOS.

<span id="paraview_oneapi_sycl">**ParaView**</span> - ParaView and VisIt do not support building SYCL kernels for VTK-m filters in released versions.

<span id="paraview_no_ospray">**ParaView**</span> - OSPRay support has been disabled due to build errors.

<span id="paraview_oneapi_python">**ParaView**</span> - Failure to build a number of Python modules with OneAPI.

<span id="sensei_ospray">**SENSEI**</span> - SENSEI is developing native OSPRay rendering support.

<span id="sensei_kokkos">**SENSEI**</span> - SENSEI is developing Kokkos support for ROCm, CUDA, and SYCL interop.

<span id="sensei_catalyst">**SENSEI**</span> - SENSEI is developing updates to support ParaView v5.11 and Catalyst 2.

<span id="visit_vtkm">**VisIt**</span> - VTK-m enabled GPU support for CUDA and ROCm is available VisIt, but is not officially tested as part of the DAV-SDK due to ([HDF5 conflict](#visit_hdf5_conflict)) only recently being resolved.

<span id="vtkm_sycl">**VTK-m**</span> - VTK-M oneAPI using SYCL.

<span id="zfp_sycl">**VTK-m**</span> - ZFP oneAPI using SYCL.

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
