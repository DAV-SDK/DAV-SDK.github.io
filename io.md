---
layout: default
---

## I/O

[back](./)

* [ADIOS2][ADIOS2]: An adaptable framework for HPC I/O supporting files, in situ,
  and in transit data movement. ADIOS2 also generates an HDF5 VOL Adapter.
* [HDF5][HDF5]: A data model, library, and file format for storing and managing
  data.
    * CUDA support (where applicable) is provided by the [HDF5 GPUDirect Storage
      VFD](https://github.com/hpc-io/vfd-gds).  Refer to the documentation for
      more information on enabling GDS VFD for your application.  The SDK will
      install the package and populate `HDF5_PLUGIN_PATH` (only).
    * [HDF5 VOL](https://docs.hdfgroup.org/hdf5/develop/group___h5_m.html)
      plugins will be installed with `HDF5_PLUGIN_PATH` populated:
        * [ADIOS2][ADIOS2]: when `ecp-data-vis-sdk +adios2 +hdf5` is installed,
          the ADIOS2 VOL is installed (by the `adios2` package).
        * [hdf5-vol-cache](https://github.com/hpc-io/vol-cache),
          [hdf5-vol-async](https://github.com/hpc-io/vol-async), and
          [hdf5-vol-log](https://github.com/DataLib-ECP/vol-log-based) are
          installed** when `ecp-data-vis-sdk +hdf5 ^hdf5@1.14:` is installed.
          ([6](#hdf5_vols_oneapi))
        * [hdf5-vol-daos](https://github.com/HDFGroup/vol-daos) is a VOL adapter
          used for direct interfacing with the Distributed Asynchronous Object
          Storage (DAOS) system, bypassing both MPI I/O and POSIX for efficient
          and scalable I/O. This VOL adapter is currently being tested on Pre-Aurora
          systems with DAOS support.
* [PNetCDF][PNetCDF]: A high-performance parallel I/O library for accessing
  Unidata's NetCDF, files in classic formats, specifically the formats of CDF-1,
   2, and 5.

[back](./)

## Notes

<span id="hdf5_vols_oneapi">**HDF5**</span> - HDF5 vols oneAPI ???.

[back](./)

[ADIOS2]: https://csmd.ornl.gov/software/adios2
[HDF5]: https://www.hdfgroup.org/solutions/hdf5/
[PNetCDF]: https://parallel-netcdf.github.io/

