## Catalyst

### Description

In Situ Analysis and Visualization represent a sea-change in the way insight is attained at the largest scales of simulation science. The gap between computing performance and I/O throughput continues to grow with the scale of HPC systems, and we are removing that bottleneck with the ParaView Catalyst platform. Catalyst provides the cleanest path to enabling in situ analysis and visualization capabilities in massively parallel simulation codes, unlocking the full power of ParaView visualization and analysis capabilities, and directly exploring simulation data in memory without ever needing to write that data to disk. Leveraging in situ analysis and visualization with Catalyst means one can visualize more time steps, analyze data more deeply, and use fewer computing resources.

Catalyst with ParaView forms the backbone of DOE’s production visualization at scale capability. Together they provide a set of C++ libraries for general-purpose visualization, a production visualization tool designed to support visualization at scale, and an in situ visualization infrastructure designed to be integrated with applications to reduce I/O overhead. Here we treat these software packages as a single entity.

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
        Catalyst with ParaView forms the backbone of DOE’s production visualization at scale capability. They are deployed at all major DOE computing facilities and are used daily for analysis and visualization. Catalyst is integrated with several DOE applications, including WarpX, MFIX, and ExaWind.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        Catalyst's next-generation capabilities with ParaView provide a range from support for accelerators to distributed visualization at scale, which are highly dependent on DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        Catalyst with ParaView has well-established quality metrics, software, and testing processes.
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
        [Catalyst][Catalyst]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][Catalyst-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][Catalyst-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][Catalyst-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[Catalyst]: https://www.paraview.org/insitu/
[Catalyst-DOC]: https://docs.paraview.org/en/latest/Catalyst/index.html
[Catalyst-REPO]: https://gitlab.kitware.com/paraview/catalyst
[Catalyst-Spack]: https://github.com/spack/spack/tree/develop/var/spack/repos/builtin/packages/libcatalyst
