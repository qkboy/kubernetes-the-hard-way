# Prerequisites

In this lab you will review the machine requirements necessary to follow this tutorial.

## Virtual or Physical Machines

This tutorial requires four (4) virtual or physical AMD64 machines running Ubuntu 20.04.1 LTS (focal). The follow table list the four machines and thier CPU, memory, and storage requirements.

| Name    | Description            | CPU | RAM   | Storage |
|---------|------------------------|-----|-------|---------|
| jumpbox | Administration host    | 1   | 512MB | 10GB    |
| server  | Kubernetes server      | 1   | 2GB   | 20GB    |
| node-0  | Kubernetes worker node | 1   | 2GB   | 20GB    |
| node-1  | Kubernetes worker node | 1   | 2GB   | 20GB    |

How you provision the machines is up to you, the only requirement is that each machine meet the above system requirements including the machine specs and OS version. Once you have all four machine provisioned, verify the system requirements by running the `uname` command on each machine:

```bash 
uname -mov
```

After running the `uname` command you should see the following output:

```text
#117~20.04.1-Ubuntu SMP Tue Apr 30 10:35:57 UTC 2024 x86_64 GNU/Linux
```

This tutorial will use `amd64` as the CPU architecture.

Next: [setting-up-the-jumpbox](02-jumpbox.md)
