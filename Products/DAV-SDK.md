## DAV-SDK

### Description

The DAV-SDK, or Data, Analysis, and Visualization Software Development Toolkit, is a comprehensive integration effort for data I/O, analysis, and visualization software developed under the Department of Energy's Advanced Scientific Computing Research program. The main product of this initiative is the DAV-SDK Spack meta-package, which combines a set of DAV SDK member packages in a way that maximizes the interoperability and features for specific environments and facilitates. The DAV SDK results from the DOE OASIS project and is supported and expanded by the DOE PESO project.

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
        We designed the DAV-SDK Spack meta-package to build and deploy a collection of DAV SDK member packages, including ADIOS, Ascent, Catalyst, DIY, HDF5, PNetCDF, ParaView, VisIt, Viskores (formerly VTK-m), and ZFP. This capability enables optimal features for specific environments and facilitates interoperability with other packages within the DAV SDK.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        We established the fundamental capabilities of DAV-SDK as a Spack meta-package. The ongoing support and development of these capabilities in updated or new systems and their application in evolving or new high-performance computing systems rely heavily on funding from the Department of Energy (DOE).
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        The DAV-SDK, while still in its early stages, benefits from quality assurance provided by Spack and the continuous integration and testing of member packages such as ADIOS, Ascent, Catalyst, DIY, HDF5, PNetCDF, ParaView, VisIt, Viskores (formerly VTK-m), and ZFP.
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
        [DAV-SDK][DAV-SDK]
      </td><!-- Website -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Documentation -->
      <td markdown="span">
        [Repository][DAV-SDK-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][DAV-SDK-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[DAV-SDK]: https://dav-sdk.github.io/
[DAV-SDK-REPO]: [https://github.com/ornladios/ADIOS2](https://github.com/DAV-SDK/davsdk)
[DAV-SDK-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/ecp-data-vis-sdk/package.py
