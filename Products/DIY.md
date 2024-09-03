## DIY

### Description

DIY is an open-source package of scalable building blocks for data movement tailored to the needs of large-scale parallel analysis and visualization workloads. Block parallelism is DIY’s parallel programming model for scalable data analysis. In this model, data are decomposed into blocks; blocks are assigned to processing elements; computation is described over these blocks, and communication between blocks is defined by reusable patterns.

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
        DIY is the ParaView, VTK, and VTK-m distributed-memory mechanism and underlies numerous other software projects such as MFA, FTK, OSUFlow, LowFive, and Tess. Since 2011, DIY supported the research of over 25 students, computer scientists, and domain scientists across 5 SciDAC projects and underpinning over 35 publications.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        DIY has sustained minimal SciDAC institute funding since it began in 2011. The fundamental capabilities of DIY are additionally supported by Kitware because DIY is a critical dependency for DOE visualization software. However, the development of next-generation features relies on sustained DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        DIY’s unit tests are executed regularly as part of Kitware’s continuous integration and regression testing. DIY includes online documentation and examples.
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
        [Documentation][DIY-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][DIY-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][DIY-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">✅</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[DIY-DOC]: https://diatomic.github.io/diy/
[DIY-REPO]: https://gitlab.kitware.com/diatomic/diy
[DIY-Spack]: https://github.com/spack/spack/tree/c3576f712d3a3abb7137d29d30c02f0c7e637122/var/spack/repos/builtin/packages/diy
