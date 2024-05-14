## VisIt

### Description

VisIt is a free, open source, platform-independent, distributed, parallel visualization tool for visualizing data defined on two- and three-dimensional structured and unstructured meshes. VisIt’s distributed architecture allows it to leverage both the compute power of a large parallel computer and the graphics acceleration hardware of a local workstation. VisIt’s user interface is often run locally on a Windows, Linux, or macOS desktop computer while its compute engine component runs in parallel on a remote computer. VisIt’s distributed architecture allows VisIt to visualize simulation data where it was generated, eliminating the need to move the data to a visualization server. VisIt can be controlled by its Graphical User Interface (GUI), through the Python and Java programming languages, or from a custom user interface you develop yourself. More information about VisIt can be found online at https://visit.llnl.gov/.

VisIt is a scalable production visualization and analysis tool widely used throughout DOE. It is designed to support visualization at scale.

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
        VisIt is widely used throughout DOE for scalable production visualization and analysis. It is deployed at all major DOE computing facilities and is used daily for analysis and visualization.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        The fundamental capabilities that VisIt provides are widely used and have a fairly sustainable funding stream. The support for ASCR compute facilities and applications is dependent on DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        VisIt has well-established quality metrics, software, and testing processes.
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
        [VisIt][VisIt]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][VisIt-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][VisIt-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][VisIt-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[VisIt]: https://visit-dav.github.io/visit-website/
[VisIt-DOC]: https://visit-sphinx-github-user-manual.readthedocs.io/en/develop/getting_help/index.html
[VisIt-REPO]: https://github.com/visit-dav/visit
[VisIt-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/visit/package.py
