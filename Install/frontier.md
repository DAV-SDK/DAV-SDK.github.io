---
layout: default
---

## Install on Frontier

[back](./)

<div style="display: flex; align-items: flex-start; gap: 20px;">
<img src="/assets/img/dav-sdk-package.png" alt="DAV SDK Package" style="width: 200px; flex-shrink: 0;">
<div>

**Note:** These are nightly deployments and are experimental.

Pre-built DAV SDK packages are deployed as environment modules on Frontier. To use them, add the module path and load the desired modules.

</div>
</div>

## Setup

Add the DAV SDK module path to your environment:

```console
$ module use /lustre/orion/world-shared/ums032/frontier-deployed-env/modules/Core
```

You can add this line to your `~/.bashrc` or job scripts to make it persistent.

## Available Modules

List available DAV SDK modules:

```console
$ module avail
```

The following modules are available:

- **adios2** - Adaptable Input/Output System
- **ascent** - In-situ visualization and analysis
- **hdf5** - Hierarchical Data Format 5
- **hdf5-vol-async** - HDF5 Asynchronous I/O VOL connector
- **hdf5-vol-cache** - HDF5 Cache VOL connector
- **libcatalyst** - Catalyst in-situ library
- **parallel-netcdf** - Parallel I/O library for NetCDF
- **paraview** - Parallel visualization application
- **vtk-m** - VTK-m visualization library
- **kokkos** - Performance portable programming model
- **zfp** - Floating-point compression library

## Loading Modules

Load a module:

```console
$ module load paraview
```

Load multiple modules:

```console
$ module load adios2 hdf5 ascent
```

Each module automatically sets the `{NAME}_ROOT` environment variable pointing to its installation prefix (e.g., `PARAVIEW_ROOT`, `ADIOS2_ROOT`).

## Example Job Script

```bash
#!/bin/bash
#SBATCH -A <project>
#SBATCH -J dav-sdk-job
#SBATCH -t 00:30:00
#SBATCH -N 1

# Load DAV SDK modules
module use /lustre/orion/world-shared/ums032/frontier-deployed-env/modules/Core
module load paraview adios2

# Run your application
srun ./my_application
```

[back](./)
