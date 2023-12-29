---
layout: default
---

## General Spack Support

[back](./)

<!-- colored tables must be done in html not markdown -->
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
        [Darshan][Darshan]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center">N/A</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
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
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center">N/A</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center">N/A</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#veloc_cuda))</td><!-- CUDA -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#veloc_rocm))</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="failing" style="text-align: center" markdown="span">([🚫](#ascent_cuda_raja))</td><!-- CUDA -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_rocm))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#ascent_no_sycl))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center">N/A</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="verified" style="text-align: center">✅</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#paraview_oneapi_sycl))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="verified" style="text-align: center" markdown="span">([✅](#sensei_ospray))</td><!-- CPU -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#sensei_kokkos))</td><!-- CUDA -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#sensei_kokkos))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#sensei_kokkos))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#visit_vtkm_support))</td><!-- CUDA -->
      <td class="verified" style="text-align: center" markdown="span">([✅](#visit_vtkm_support))</td><!-- ROCm -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#visit_vtkm_support))</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="verified" style="text-align: center">✅</td><!-- ROCm -->
      <td class="verified" style="text-align: center">✅</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="na" style="text-align: center">N/A</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [cuSZ][cuSZ]
      </td>
      <td class="na" style="text-align: center">N/A</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="na" style="text-align: center">N/A</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- CPU -->
      <td class="verified" style="text-align: center">✅</td><!-- CUDA -->
      <td class="na" style="text-align: center" markdown="span">([N/A](#zfp_rocm))</td><!-- ROCm -->
      <td class="na" style="text-align: center">N/A</td><!-- SYCL -->
    </tr>
  </tbody>
</table>

[back](./)
