# Clara DICOM Adapter

[![NVIDIA](https://docs.nvidia.com/clara/images/clara_deploy_image.png)](https://docs.nvidia.com/clara/deploy/index.html)


Designed for the Clara Deploy SDK, the Clara DICOM Adapter implements the
necessary DICOM services for interoperability between Clara and other medical
devices. The Clara DICOM Adapter allows you to send/receive DICOM objects
using standard DICOM protocols and interpret standard DICOM part-10 formats.

## Additional Resources to Learn More on Clara Deploy

* [NVIDIA Clara Overview Homepage](https://developer.nvidia.com/clara)
* [NVIDIA Clara Deploy SDK User Guide](https://docs.nvidia.com/clara/deploy/index.html)

## Build

### Prerequisites

* [.NET Core 3.1 SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1)
* DCMTK (Required for running integration test)


### Development Environment

DICOM Adapter follows the [Generic Host](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/host/generic-host?view=aspnetcore-3.1) design with .NET Core.  In order to for it to pickup `appsettings.Development.json` 
you must export the following environment variable before executing `dotnet run`:

```bash
export DOTNETCORE_ENVIRONMENT=Development
```


### Building Clara DICOM Adapter

```bash
src$ dotnet build
```

### Building Clara DICOM Adapter Docker Container

```bash
src$ ./build.sh
```

### Running Unit Test

```bash
src$ dotnet test
```

## Coding Guidelines
* [C# coding style](coding-style.md)

## Licenses
### [NVIDIA License](LICENSE)
### [Individual Contributor License Agreement](https://www.apache.org/licenses/icla.pdf)
### [Open Source Licenses](LICENSE-3rdParty)
