## PNetCDF

### Description

PnetCDF is a high-level library providing parallel and scalable access to Unidata's NetCDF files. The data model defined in the netCDF files supports abstraction for storing and retrieving multidimensional data and associated attributes in a portable format across platforms. PnetCDF is widely used in the climate and weather communities, as the Intergovernmental Panel on Climate Change (IPCC) has mandated the netCDF format for storing climate-related data since 2005.
### Impact, Sustainability, and Quality

<table class="isq_table">
  <thead>
    <tr>
      <th>Property</th>
      <th style="text-align: center">State</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <strong>Impact</strong>
      </td>
      <td>
        Deployed on all DOE HPC machines, PnetCDF is widely used across climate research and weather forecasting communities. Well-known DOE applications include E3SM, ExaWind, SPARC, and EMPIRE. Outside of DOE, PnetCDF is also used in WRF/CESM/CAM supported by NSF, NVIDIA, NOAA, HPE/Cray, General Atomics, and EPA.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        PnetCDF, as an open-source software, has been supported by the SciDAC office since 2001. It has a well-established system for user support and code contribution. PnetCDF follows a standard contiguous integration process, using a comprehensive set of test programs and software release mechanisms developed in the past.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        PnetCDF is routinely tested on DOE parallel computers. The developer team constantly creates case studies based on the application’s I/O kernel, which are used for verification, validation, and educational purposes.
      </td>
    </tr>
  </tbody>
</table>

### Software Quality Characteristics

<table class="status_table">
  <thead>
    <tr>
      <th style="text-align: center">Website</th>
      <th style="text-align: center">Documentation</th>
      <th style="text-align: center">Repository</th>
      <th style="text-align: center">Test Suite</th>
      <th style="text-align: center">Spack</th>
      <th style="text-align: center">E4S</th>
      <th style="text-align: center">Smoke Test</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td markdown="span">
        [PNetCDF][PNetCDF]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][PNetCDF-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][PNetCDF-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][PNetCDF-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">✅</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[PNetCDF]: https://parallel-netcdf.github.io
[PNetCDF-DOC]: https://parallel-netcdf.github.io/wiki/Documentation.html
[PNetCDF-REPO]: https://github.com/Parallel-NetCDF/PnetCDF
[PNetCDF-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/parallel-netcdf/package.py
