# VCPKG Template
Template for adding external libraries to C++ project using VCPKG

Before making the project you need to configure the `VCPKG_ROOT` environment variable:

```PowerShell
$env:VCPKG_ROOT = "C:\path\to\vcpkg"
$env:PATH = "$env:VCPKG_ROOT;$env:PATH"
```

To add a dependencies use: 
```PowerShell
vcpkg add port <package>
```

You need to have vcpkg and cmake installed before that. Specify the path of the vcpkg folder in `CMakeUserPresets.json`