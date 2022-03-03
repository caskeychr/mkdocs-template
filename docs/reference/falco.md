# Falco

The Falco Project, originally created by Sysdig, is an incubating CNCF open source cloud native runtime security tool. Falco makes it easy to consume kernel events, and enrich those events with information from Kubernetes and the rest of the cloud native stack. Falco has a rich set of security rules specifically built for Kubernetes, Linux, and cloud-native. If a rule is violated in a system, Falco will send an alert notifying the user of the violation and its severity.

## What can Falco detect?

Falco can detect and alert on any behavior that involves making Linux system calls. Falco alerts can be triggered by the use of specific system calls, their arguments, and by properties of the calling process. For example, Falco can easily detect incidents including but not limited to:

- A shell is running inside a container or pod in Kubernetes.
- A container is running in privileged mode, or is mounting a sensitive path, such as /proc, from the host.
- A server process is spawning a child process of an unexpected type.
- Unexpected read of a sensitive file, such as /etc/shadow.
- A non-device file is written to /dev.
- A standard system binary, such as ls, is making an outbound network connection.
- A privileged pod is started in a Kubernetes cluster.

Additional Documentation: [Click Here](https://github.com/falcosecurity/falco)
