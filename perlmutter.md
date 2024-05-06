---
layout: default
---

## Perlmutter Support

[back](./)

## Toolchains

One of the primary challenges on Perlmutter is handling the compiler wrapper
for the NVHPC compilers, in particular how they wrap MPI and CUDA.

<table class="toolchain_table">
  <thead>
    <tr>
      <th>Info</th>
      <th style="text-align: center">GCC Toolchain</th>
      <th style="text-align: center">NVHPC Toolchain</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        Version
      </td>  <!-- Info -->
      <td style="text-align: center">v11.2</td>  <!-- GCC Toolchain -->
      <td style="text-align: center">v22.4</td>  <!-- NVHPC Toolchain -->
    </tr>
    <tr>
      <td>
        Cray MPICH
      </td>  <!-- Info -->
      <td style="text-align: center">v8.2.3</td>  <!-- GCC Toolchain -->
      <td style="text-align: center">v8.2.3</td>  <!-- NVHPC Toolchain -->
    </tr>
    <tr>
      <td>
        CUDA
      </td>  <!-- Info -->
      <td style="text-align: center">v11.3</td>  <!-- GCC Toolchain -->
      <td style="text-align: center">v11.3</td>  <!-- NVHPC Toolchain -->
    </tr>
  </tbody>
</table>

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th style="text-align: center">GCC</th>
      <th style="text-align: center">GCC + CUDA</th>
      <th style="text-align: center">NVHPC + CUDA</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="na" style="text-align: center">N/A</td><!-- GCC + CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="failing" style="text-align: center" markdown="span">([🚫](#ascent_cuda_raja) [🚫](#ascent_perlmutter_mpi))</td><!-- GCC + CUDA -->
      <td class="failing" style="text-align: center" markdown="span">([🚫](#ascent_cuda_raja) [🚫](#ascent_perlmutter_mpi))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [DIY][DIY]
      </td>
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- GCC -->
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- GCC + CUDA -->
      <td class="na" style="text-align: center" markdown="span">([🔎](#diy))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#paraview_cuda))</td><!-- GCC + CUDA -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#paraview_cuda))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="in_progress" style="text-align: center" markdown="span">🔎</td><!-- GCC -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#visit_vtkm))</td><!-- GCC + CUDA -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#visit_vtkm))</td><!-- NVHPC + CUDA -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center" markdown="span">✅</td><!-- GCC -->
      <td class="verified" style="text-align: center">✅</td><!-- GCC + CUDA -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#vtkm_nvhpc))</td><!-- NVHPC + CUDA -->
    </tr>
  </tbody>
</table>

<p style="text-align:center; border-width:3px; border-style:solid; border-color:#4393c3; padding: 0.5em;">✅ - <b>Verified</b>&emsp;🔎 - <b>In Progress</b>&emsp;🚫 - <b>Broken</b>&emsp;N/A - <b>Not Applicable</b></p>

[back](./)

## Notes

<span id="ascent_cuda_raja">**Ascent**</span> - Blocked by build errors in RAJA package.

<span id="ascent_perlmutter_mpi">**Ascent**</span> - The way MPI is set up on Perlmutter conflicts with Ascent's spack recipe and CMake. Fixes for this are being developed.

<span id="diy">**DIY**</span> - Not yet in DAV SDK.

<span id="paraview_cuda">**ParaView**</span> - ParaView VTK-m using CUDA.

<span id="visit_hdf5_conflict">**VisIt**</span> - VisIt utilizes a VTK version locked to a Python that is not compatible with the Python requirements of PyH5, the HDF5 python interface used by Cinema.

<span id="visit_vtkm">**VisIt**</span> - VTK-m enabled GPU support for CUDA and ROCm is available VisIt, but is not officially tested as part of the DAV-SDK due to ([HDF5 conflict](#visit_hdf5_conflict)) only recently being resolved.

<span id="vtkm_nvhpc">**VTK-m**</span> - VTK-M NVHPC using CUDA.

<span id="zfp_nvhpc">**VTK-m**</span> - VTK-M NVHPC using CUDA.

[back](./)

[ADIOS2]: https://csmd.ornl.gov/software/adios2
[HDF5]: https://www.hdfgroup.org/solutions/hdf5/
[Ascent]: https://github.com/Alpine-DAV/ascent
[DIY]: https://gitlab.kitware.com/diatomic/diy
[ParaView]: https://paraview.org
[VisIt]: https://visit-dav.github.io/visit-website/
[VTK-m]: https://m.vtk.org
