---
layout: default
---

## DAV SDK Support

[back](./)

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th style="text-align: center">CPU</th>
      <th style="text-align: center">CUDA</th>
      <th style="text-align: center">ROCm</th>
      <th style="text-align: center" markdown="span">([SYCL](#oneapi_sycl))</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#adios2_rocm))</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="failing" style="text-align: center" markdown="span">([🚫](#ascent_cuda))</td><!-- CUDA -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_rocm))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#ascent_sycl))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [DIY][DIY]
      </td>
      <td class="na" style="text-align: center" markdown="span">✅</td><!-- CPU -->
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- CUDA -->
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="verified" style="text-align: center">✅</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#paraview_sycl))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#visit_vtkm))</td><!-- CUDA -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#visit_vtkm))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#visit_sycl))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="verified" style="text-align: center">✅</td><!-- ROCm -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- SYCL -->
    </tr>
  </tbody>
</table>

<p style="text-align:center; border-width:3px; border-style:solid; border-color:#4393c3; padding: 0.5em;">✅ - <b>Verified</b>&emsp;🔎 - <b>In Progress</b>&emsp;🚫 - <b>Broken</b>&emsp;N/A - <b>Not Applicable</b></p>

[back](./)

## Notes

<span id="oneapi_sycl">**SYCL**</span> - [SYCL](https://www.khronos.org/sycl/) extensions are implemented and tested using [oneAPI](https://www.intel.com/content/www/us/en/developer/tools/oneapi/overview.html).

<span id="adios2_rocm">**ADIOS2**</span> - ADIOS2 ROCm/HIP support is not expected in near term release.

<span id="ascent_cuda">**Ascent**</span> - Ascent CUDA blocked by build errors in RAJA package.

<span id="ascent_rocm">**Ascent**</span> - Ascent spack recipe does not have support for ROCm. It is in under development in the Alpine Spack fork.

<span id="ascent_sycl">**Ascent**</span> - Ascent currently does not have any known plans for explicit SYCL support.

<span id="diy">**DIY**</span> - Not yet in DAV SDK.

<span id="paraview_sycl">**ParaView**</span> - ParaView using oneAPI does not support building SYCL kernels for VTK-m filters in released versions.

<span id="visit_hdf5_conflict">**VisIt**</span> - VisIt utilizes a VTK version locked to a Python that is not compatible with the Python requirements of PyH5, the HDF5 python interface used by Cinema.

<span id="visit_vtkm">**VisIt**</span> - VTK-m enabled GPU support for CUDA and ROCm is available VisIt, but is not officially tested as part of the DAV-SDK due to ([HDF5 conflict](#visit_hdf5_conflict)) only recently being resolved.

<span id="visit_sycl">**VisIt**</span> - VisIt using oneAPI does not support building SYCL kernels for VTK-m filters in released versions.

[back](./)

[ADIOS2]: https://csmd.ornl.gov/software/adios2
[HDF5]: https://www.hdfgroup.org/solutions/hdf5/
[Ascent]: https://github.com/Alpine-DAV/ascent
[DIY]: https://gitlab.kitware.com/diatomic/diy
[ParaView]: https://paraview.org
[VisIt]: https://visit-dav.github.io/visit-website/
[VTK-m]: https://m.vtk.org
