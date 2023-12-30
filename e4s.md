---
layout: default
---

## Extreme-scale Scientific Software Stack (E4S) Support

This table is an overview of the status of the different CPU-only deployments of the DAV SDK via E4S. Some items may be marked as "🔎" but may have fully completed some tasks on those systems.

[back](./)

<table class="status_table">
  <thead>
    <tr>
      <th>Project</th>
      <th style="text-align: center">Desktop</th>
      <th style="text-align: center">Docker</th>
      <th style="text-align: center">Frontier</th>
      <th style="text-align: center">Perlmutter</th>
      <th style="text-align: center" markdown="span">([Aurora](#verified_on_sunspot))</th>
      <th style="text-align: center">Smoke</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [ADIOS2][ADIOS2]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [Darshan][Darshan]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [HDF5][HDF5]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#hdf5_vols_oneapi))</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [UnifyFS][UnifyFS]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [VeloC][VeloC]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [Ascent][Ascent]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#ascent_find_mpi_frontier))</td><!-- Frontier -->
      <td class="failing" style="text-align: center" markdown="span">([🚫](#ascent_perlmutter_mpi))</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [Cinema][Cinema]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#cinema_oneapi_python))</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [ParaView][ParaView]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#paraview_no_ospray)[🔎](#paraview_oneapi_python))</td><!-- Aurora -->
      <td class="verified" style="text-align: center">✅</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [SENSEI][SENSEI]
      </td>
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- Desktop -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- Docker -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- Frontier -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center" markdown="span">([🔎](#sensei_catalyst))</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [VisIt][VisIt]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [VTK-m][VTK-m]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Aurora -->
      <td class="verified" style="text-align: center">✅</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [SZ][SZ]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [cuSZ][cuSZ]
      </td>
      <td class="na" style="text-align: center">N/A</td><!-- Desktop -->
      <td class="na" style="text-align: center">N/A</td><!-- Docker -->
      <td class="na" style="text-align: center">N/A</td><!-- Frontier -->
      <td class="na" style="text-align: center">N/A</td><!-- Perlmutter -->
      <td class="na" style="text-align: center">N/A</td><!-- Aurora -->
      <td class="na" style="text-align: center">N/A</td><!-- Smoke -->
    </tr>
    <tr>
      <td markdown="span">
        [ZFP][ZFP]
      </td>
      <td class="verified" style="text-align: center">✅</td><!-- Desktop -->
      <td class="verified" style="text-align: center">✅</td><!-- Docker -->
      <td class="verified" style="text-align: center">✅</td><!-- Frontier -->
      <td class="verified" style="text-align: center">✅</td><!-- Perlmutter -->
      <td class="verified" style="text-align: center">✅</td><!-- Aurora -->
      <td class="in_progress" style="text-align: center">🔎</td><!-- Smoke -->
    </tr>
  </tbody>
</table>

<p style="text-align:center; border-width:3px; border-style:solid; border-color:#4393c3; padding: 0.5em;">✅ - <b>Verified</b>&emsp;🔎 - <b>In Progress</b>&emsp;🚫 - <b>Broken</b>&emsp;N/A - <b>Not Applicable</b></p>

[back](./)

## Notes

<span id="verified_on_sunspot">**Aurora**</span> - Due to the similarity between the toolchains on Aurora and Sunspot, the results for the Aurora system are currently marked as verified as builds on Aurora progress. As issues are found on Aurora, these values will be updated to reflect the target system status.

<span id="ascent_perlmutter_mpi">**Ascent**</span> - The way MPI is set up on Perlmutter conflicts with Ascent's spack recipe and CMake. Fixes for this are being developed.

<span id="ascent_find_mpi_frontier">**Ascent**</span> - Using the CCE toolchain has issues locating MPI with CMake.

<span id="cinema_oneapi_python">**Cinema**</span> - Failure to build a number of Python modules with OneAPI.

<span id="hdf5_vols_oneapi">**HDF5**</span> - HDF5 vols oneAPI ???.

<span id="paraview_no_ospray">**ParaView**</span> - OSPRay support has been disabled due to build errors.

<span id="paraview_oneapi_python">**ParaView**</span> - Failure to build a number of Python modules with OneAPI.

<span id="sensei_catalyst">**SENSEI**</span> - SENSEI is developing updates to support ParaView v5.11 and Catalyst 2.

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
