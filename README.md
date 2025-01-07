# 🔧 .NET Kubectl CLI

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Test](https://github.com/devantler/dotnet-kubectl-cli/actions/workflows/test.yaml/badge.svg)](https://github.com/devantler/dotnet-kubectl-cli/actions/workflows/test.yaml)
[![codecov](https://codecov.io/gh/devantler/dotnet-kubectl-cli/graph/badge.svg?token=RhQPb4fE7z)](https://codecov.io/gh/devantler/dotnet-kubectl-cli)

<details>
  <summary>Show/hide folder structure</summary>

<!-- readme-tree start -->
```
.
├── .github
│   ├── scripts
│   └── workflows
├── Devantler.KubectlCLI
│   └── runtimes
│       ├── linux-arm64
│       │   └── native
│       ├── linux-x64
│       │   └── native
│       ├── osx-arm64
│       │   └── native
│       ├── osx-x64
│       │   └── native
│       ├── win-arm64
│       │   └── native
│       └── win-x64
│           └── native
└── Devantler.KubectlCLI.Tests
    └── KubectlTests

19 directories
```
<!-- readme-tree end -->

</details>

A simple .NET library that embeds the Kubectl CLI.

## 🚀 Getting Started

To get started, you can install the package from NuGet.

```bash
dotnet add package Devantler.KubectlCLI
```

## 📝 Usage

You can execute the Kubectl CLI commands using the `Kubectl` class.

```csharp
using Devantler.KubectlCLI;

var (exitCode, message) = await Kubectl.RunAsync(["arg1", "arg2"]);
```
