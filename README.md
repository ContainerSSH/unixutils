[![ContainerSSH - Launch Containers on Demand](https://containerssh.github.io/images/logo-for-embedding.svg)](https://containerssh.github.io/)

<!--suppress HtmlDeprecatedAttribute -->
<h1 align="center">ContainerSSH UNIX Utilities Library</h1>

[![Go Report Card](https://goreportcard.com/badge/github.com/containerssh/unixutils?style=for-the-badge)](https://goreportcard.com/report/github.com/containerssh/unixutils)
[![LGTM Alerts](https://img.shields.io/lgtm/alerts/github/ContainerSSH/unixutils?style=for-the-badge)](https://lgtm.com/projects/g/ContainerSSH/unixutils/)

This library contains UNIX and Linux related utilities for ContainerSSH

<p align="center"><strong>Note: This is a developer documentation.</strong><br />The user documentation for ContainerSSH is located at <a href="https://containerssh.github.io">containerssh.github.io</a>.</p>

## ParseCMD

The `ParseCMD()` method takes a command line and parses it into an execv-compatible slice of strings.

```go
args, err := unixutils.ParseCMD("/bin/sh -c 'echo \"Hello world!\"'")
//args will be: ["/bin/sh", "-c", "echo \"Hello world!\"]
```
