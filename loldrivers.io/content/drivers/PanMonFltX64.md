+++
description = "https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-driver-block-rules"
title = "PanMonFltX64.sys"
weight = 10
+++

# PanMonFltX64.sys

#### Description

CapCom.sys is a vulnerable driver that has been abused over the years.

- **Created**: 2023-01-09
- **Author**: Michael Haag
- **Acknowledgement**:  | [](https://twitter.com/)

#### Command

```
sc create CapCom binpath = c:\temp\capcom.sys type=kernel start=auto displayname="CapCom vulnerable Driver"
```

#### Resources


- {&#39; https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-driver-block-rules&#39;}





#### Binary Metadata

- Known Hashes: [](https://www.virustotal.com/gui/file/) 
- binary: 
- Verified: 
- Date: 
- Publisher: 
- Company: 
- Description: 
- Product: 
- ProductVersion: 
- FileVersion: 
- MachineType: 
- OriginalFilename: 

[*source*](https://github.com/magicsword-io/LOLDrivers/tree/main/yaml/panmonfltx64.sys.yml)