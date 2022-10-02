[![ContainerSSH - Launch Containers on Demand](https://containerssh.github.io/images/logo-for-embedding.svg)](https://containerssh.github.io/)

<!--suppress HtmlDeprecatedAttribute -->
<h1 align="center">ContainerSSH UNIX Utilities Library</h1>

<p align="center"><strong>⚠⚠⚠ Deprecated: ⚠⚠⚠</strong><br />This repository is deprecated in favor of <a href="https://github.com/ContainerSSH/libcontainerssh">libcontainerssh</a> for ContainerSSH 0.5.</p>

This library contains UNIX and Linux related utilities for ContainerSSH

## ParseCMD

The `ParseCMD()` method takes a command line and parses it into an execv-compatible slice of strings.

```go
args, err := unixutils.ParseCMD("/bin/sh -c 'echo \"Hello world!\"'")
//args will be: ["/bin/sh", "-c", "echo \"Hello world!\"]
```
