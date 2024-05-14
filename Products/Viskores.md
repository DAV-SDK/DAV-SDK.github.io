## Viskores (formerly know as VTK-m)

### Description

Viskores is a toolkit of scientific visualization algorithms for emerging processor architectures. It supports the fine-grained concurrency for data analysis and visualization algorithms required to drive extreme-scale computing by providing abstract models for data and execution that can be applied to a variety of algorithms across many different processor architectures.

Viskores provides the fundamental capability to execute visualization algorithms on Exascale hardware and, by extension, HPC platforms of most scales. More specifically, Viskores operates on GPU and other accelerator processors that rely on an extreme amount of lightweight thread parallelism to perform efficiently. Viskores is designed with an abstract compute model and portability in mind to allow it to operate on GPUs and other multiple-core devices such as multi-core CPUs and potential future processor designs.

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
        Viskores is the common solution for implementing visualization algorithms on GPU processors. The software can take advantage of the readily available visualization algorithms provided by VTK-m. ParaView and VisIt, the premier DOE visualization tools, are integrating Viskores into their products today. A growing list of GPU-enabled algorithms is replacing the underlying data processing. Likewise, the Ascent in situ library uses Viskores exclusively for its data processing infrastructure.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Sustainability</strong>
      </td>
      <td>
        Through the exascale computing project (ECP), Viskores has made important progress in providing a production-worthy software base. Additionally, Viskores has been updated to demonstrate use on both Frontier and Aurora, and it has been applied to multiple application problems. However, although much progress was made during ECP for functionality and general portability, the later availability of early access and Exascale hardware has left room for targeted improvements on these and other platforms. There is no funding outside of OASIS for these activities.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Quality</strong>
      </td>
      <td>
        Viskores has well-established software management, contribution, and testing processes. Consumers of Viskores rely on regular releases, which must be maintained by the team.
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
        [Viskores][Viskores]
      </td><!-- Website -->
      <td markdown="span">
        [Documentation][Viskores-DOC]
      </td><!-- Documentation -->
      <td markdown="span">
        [Repository][Viskores-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td markdown="span">
        [Spack][Viskores-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">✅</td><!-- Smoke Test -->
    </tr>
  </tbody>
</table>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to demonstrate how project efforts lead to measurable increases in software quality.

[Viskores]: https://m.vtk.org/
[Viskores-DOC]: https://Viskores.readthedocs.io/en/v2.10.0/
[Viskores-REPO]: https://github.com/ornladios/Viskores
[Viskores-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/vtk-m/package.py
