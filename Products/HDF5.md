## HDF5

### Description

HDF5 is a self-describing, portable, and hierarchical file format designed for high-performance I/O and featuring various integrated features that can help optimize storage space and access time. Because it can optimize system-tailored I/O at scale, HDF5 is widely used by industry, academic, and government organizations. It's also highly compatible with other systems, making data sharing, collaboration, and analysis quick and trouble-free.

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
        The HDF5 library is crucial for the large-scale data input/output process of the DOE. It is extensively used at all DOE computing facilities and relied upon by other I/O standards, libraries, and DOE research applications.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        HDF has been developed for 25 years with significant government funding. This funding is used for new feature development, maintenance, documentation, and testing at DOE computing facilities.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        The HDF5 library has well-established quality metrics, software, and testing processes.
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
        [HDF5][HDF5]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][HDF5-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][HDF5-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][HDF5-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[HDF5]: https://www.hdfgroup.org/solutions/hdf5/
[HDF5-DOC]: https://portal.hdfgroup.org/documentation/
[HDF5-REPO]: https://github.com/HDFGroup/hdf5
[HDF5-Spack]: https://github.com/spack/spack/tree/c3576f712d3a3abb7137d29d30c02f0c7e637122/var/spack/repos/builtin/packages/hdf5
