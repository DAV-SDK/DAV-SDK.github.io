## ADIOS

### Description

ADIOS, the Adaptable Input/Output (I/O) System, transports data as groups of self-describing variables and attributes across different media types (such as files, wide-area networks, and remote direct memory access) using a common application programming interface for all transport modes. ADIOS focuses on I/O scalable performance, adaptability, and ease of use.

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
        **Impact**
      </td>
      <td>
        ADIOS is a scalable I/O solution that provides high I/O performance for applications from a single computer to exascale supercomputers. It is deployed at all major DOE compute facilities and used by high-profile applications in their daily production runs, including a number of DOE applications, such as WarpX, ImpactX, XGC, GENE, GEM, E3SM, S3D, Bout++, and GTC, and other data-intensive applications, like SPECFEM3D_GLOBE, PIConGPU, GE Research’ CFD simulation, TAE fusion simulations, etc.
      </td>
    </tr>
    <tr>
      <td>
        **Sustainability**
      </td>
      <td>
        ADIOS's fundamental capabilities are file-based storage I/O and various in situ data transfers, namely in memory, in the system, and in wide-area-network staging. The continued support of these capabilities in updated or new systems and evolving or new applications is highly dependent on DOE funding.
      </td>
    </tr>
    <tr>
      <td>
        **Quality**
      </td>
      <td>
        ADIOS has well-established software management and testing processes, including public repository, bug tracking, documentation, and CI processes for many platforms.
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
      <td>
        [ADIOS2][ADIOS2]
      </td><!-- Website -->
      <td>
        [Documentation][ADIOS2-DOC]
      </td><!-- Documentation -->
      <td>
        [Repository][ADIOS2-REPO]
      </td><!-- Repository -->
      <td style="text-align: center" markdown="span">✅</td><!-- Test Suite -->
      <td>
        [Spack][ADIOS2-Spack]
      </td><!-- Spack -->
      <td style="text-align: center" markdown="span">✅</td><!-- E4S -->
      <td style="text-align: center" markdown="span">🚫</td><!-- Smoke Test -->
    </tr>
  </tbody>

**Note**: Working with the OASIS leadership to refine metrics and identify methods to clearly demonstrate how project efforts lead to measurable increases in software quality.

[ADIOS2]: https://csmd.ornl.gov/software/adios2
[ADIOS2-DOC]: https://adios2.readthedocs.io/en/v2.10.0/
[ADIOS2-REPO]: https://github.com/ornladios/ADIOS2
[ADIOS2-Spack]: https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/adios2/package.py
</table>
