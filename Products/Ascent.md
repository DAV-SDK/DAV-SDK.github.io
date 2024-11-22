## Ascent

### Description

Ascent is a many-core capable flyweight in situ visualization and analysis infrastructure for multi-physics HPC simulations.

The Ascent in situ infrastructure is designed for leading-edge supercomputers and supports both distributed-memory and shared-memory parallelism. Ascent can take advantage of computing power on conventional CPU architectures and on many-core architectures such as NVIDIA and AMD GPUs. Further, it has a flexible design that supports the integration of new visualization and analysis routines and libraries.

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
        Ascent is integrated with several DOE applications, including WarpX, Nyx, and AMR-Wind. It is deployed at all major DOE computing facilities and is used daily for analysis and visualization.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        Ascent's fundamental capabilities are widely used, and it has a fairly sustainable DOE NNSA funding stream. The support for ASCR computing facilities and applications is dependent on DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        Ascent has well-established quality metrics, software, and testing processes.
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
      <td style="text-align: center" markdown="span">✅</td><!-- Website -->
      <td markdown="span">
        [Documentation][Ascent-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][Ascent-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][Ascent-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">✅</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[Ascent-DOC]: https://ascent.readthedocs.io/
[Ascent-REPO]: https://github.com/Alpine-DAV/ascent
[Ascent-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/ascent/package.py
