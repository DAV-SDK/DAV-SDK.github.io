## ParaView

### Description

ParaView is an open-source, multi-platform data analysis and visualization application based on the Visualization Toolkit (VTK).

ParaView and Catalyst form the backbone of DOE’s production visualization at scale capability. Together they provide a set of C++ libraries for general-purpose visualization, a production visualization tool designed to support visualization at scale, and an in situ visualization infrastructure designed to be integrated with applications to reduce I/O overhead.

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
        ParaView forms the backbone of DOE’s production visualization at scale capability. It is deployed at all major DOE computing facilities and is used daily for analysis and visualization. 
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        The fundamental capabilities that ParaView provides are widely used and have a fairly sustainable funding stream. On the other hand, the next-generation capabilities that ParaView provides, ranging from support for accelerators to distributed visualization at scale, are highly dependent on DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        ParaView has well-established quality metrics, software, and testing processes.
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
        [ParaView][ParaView]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][ParaView-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][ParaView-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][ParaView-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">✅</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[ParaView]: https://www.paraview.org/
[ParaView-DOC]: https://www.paraview.org/resources/
[ParaView-REPO]: https://gitlab.kitware.com/paraview/paraview
[ParaView-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/paraview/package.py
