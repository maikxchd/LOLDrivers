+++

description = ""
title = "50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3"
weight = 10

+++


{{< block "grid-1" >}}
{{< column "mt-2 pt-1">}}


# mhyprot.sys ![:inline](/images/twitter_verified.png) 


### Description

mhyprot.sys is a driver associated with the anticheat software used by the gaming company miHoYo.
- **UUID**: 50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3
- **Created**: 2023-01-09
- **Author**: Michael Haag
- **Acknowledgement**:  | [](https://twitter.com/)

{{< button "https://github.com/magicsword-io/LOLDrivers/raw/main/drivers/4b817d0e7714b9d43db43ae4a22a161e.bin" "Download" >}}
{{< tip "warning" >}}
This download link contains the vulnerable driver!

{{< /tip >}}

### Commands

```
sc.exe create mhyprot.sys binPath=C:\windows\temp\mhyprot.sys type=kernel &amp;&amp; sc.exe start mhyprot.sys
```

| Use Case | Privileges | Operating System | 
|:---- | ---- | ---- |
| Elevate privileges | kernel | Windows 10 |

### Resources
<br>
<li><a href=" https://github.com/jbaines-r7/dellicious"> https://github.com/jbaines-r7/dellicious</a></li>
<li><a href=" https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/"> https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/</a></li>
<li><a href="https://github.com/elastic/protections-artifacts/blob/932baf346cc8a743f1963ad3d4565b42ed17bebe/yara/rules/Windows_VulnDriver_Mhyprot.yar">https://github.com/elastic/protections-artifacts/blob/932baf346cc8a743f1963ad3d4565b42ed17bebe/yara/rules/Windows_VulnDriver_Mhyprot.yar</a></li>
<li><a href="https://github.com/jbaines-r7/dellicious and https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/">https://github.com/jbaines-r7/dellicious and https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/</a></li>
<br>

### Known Vulnerable Samples

| Property           | Value |
|:-------------------|:------|
| Filename           | mhyprot.sys |
| MD5                | [4b817d0e7714b9d43db43ae4a22a161e](https://www.virustotal.com/gui/file/4b817d0e7714b9d43db43ae4a22a161e) |
| SHA1               | [0466e90bf0e83b776ca8716e01d35a8a2e5f96d3](https://www.virustotal.com/gui/file/0466e90bf0e83b776ca8716e01d35a8a2e5f96d3) |
| SHA256             | [509628b6d16d2428031311d7bd2add8d5f5160e9ecc0cd909f1e82bbbb3234d6](https://www.virustotal.com/gui/file/509628b6d16d2428031311d7bd2add8d5f5160e9ecc0cd909f1e82bbbb3234d6) |
| Authentihash MD5   | [ff295de93e6b6dcc3938d50901a7240d](https://www.virustotal.com/gui/search/authentihash%253Aff295de93e6b6dcc3938d50901a7240d) |
| Authentihash SHA1  | [484c72dd4fd91083b249f3ccc733a3c8335e583f](https://www.virustotal.com/gui/search/authentihash%253A484c72dd4fd91083b249f3ccc733a3c8335e583f) |
| Authentihash SHA256| [0c7809ac1fa074408518ddc0ac118912c9cd43ed9c89213bc4d59043016b040c](https://www.virustotal.com/gui/search/authentihash%253A0c7809ac1fa074408518ddc0ac118912c9cd43ed9c89213bc4d59043016b040c) |


#### Imports
{{< details "Expand" >}}
* ntoskrnl.exe
* WDFLDR.SYS

{{< /details >}}
#### ImportedFunctions
{{< details "Expand" >}}
* NtQuerySystemInformation
* RtlInitUnicodeString
* ExAllocatePool
* ExAllocatePoolWithTag
* ExFreePoolWithTag
* IofCompleteRequest
* IoCreateDevice
* IoCreateSymbolicLink
* IoDeleteDevice
* IoDeleteSymbolicLink
* _wcsicmp
* RtlInitString
* RtlAnsiStringToUnicodeString
* RtlFreeUnicodeString
* IoGetDeviceObjectPointer
* ZwClose
* MmIsAddressValid
* ZwOpenDirectoryObject
* ZwQueryDirectoryObject
* ObReferenceObjectByName
* ZwQuerySystemInformation
* __C_specific_handler
* MmHighestUserAddress
* IoDriverObjectType
* KeQueryTimeIncrement
* KeStackAttachProcess
* KeUnstackDetachProcess
* PsGetProcessWow64Process
* PsGetProcessPeb
* MmUnlockPages
* MmGetSystemRoutineAddress
* MmUnmapLockedPages
* IoFreeMdl
* ZwTerminateProcess
* PsGetProcessImageFileName
* ObOpenObjectByPointer
* PsReferenceProcessFilePointer
* IoQueryFileDosDeviceName
* ZwQueryVirtualMemory
* MmProbeAndLockPages
* PsLookupProcessByProcessId
* MmMapLockedPagesSpecifyCache
* IoAllocateMdl
* IoGetCurrentProcess
* MmCopyVirtualMemory
* KeClearEvent
* KeSetEvent
* KeWaitForSingleObject
* MmMapLockedPages
* ObReferenceObjectByHandle
* PsSetCreateProcessNotifyRoutineEx
* PsSetCreateThreadNotifyRoutine
* PsRemoveCreateThreadNotifyRoutine
* PsSetLoadImageNotifyRoutine
* PsRemoveLoadImageNotifyRoutine
* ExEventObjectType
* ObRegisterCallbacks
* ObUnRegisterCallbacks
* ObGetFilterVersion
* IoThreadToProcess
* strcmp
* PsProcessType
* PsThreadType
* RtlGetVersion
* ObfReferenceObject
* ObGetObjectType
* ExEnumHandleTable
* ExfUnblockPushLock
* _snprintf
* vsprintf_s
* ZwCreateFile
* ZwWriteFile
* PsLookupThreadByThreadId
* NtQueryInformationThread
* PsGetThreadProcess
* DbgPrint
* KeDelayExecutionThread
* KdDisableDebugger
* KdChangeOption
* PsCreateSystemThread
* PsTerminateSystemThread
* KdDebuggerEnabled
* PsGetVersion
* KeInitializeEvent
* RtlCopyUnicodeString
* ObfDereferenceObject
* ExReleaseFastMutex
* ExAcquireFastMutex
* MmBuildMdlForNonPagedPool
* WdfVersionBindClass
* WdfVersionBind
* WdfVersionUnbind
* WdfVersionUnbindClass

{{< /details >}}
#### ExportedFunctions
{{< details "Expand" >}}

{{< /details >}}

#### Signature
{{< details "Expand" >}}
```
{
  "Certificates": [
    {
      "Signature": "46a5e6f6c38a63b314f7e2677bb86d4bcd7839eef8e006048ddd58c6783ff0657456e61c800efb31966c611f7ca7d1de1785e006e3f4c0b24cb652842e42cbae016320a774724537fc30e8f09895fdb626daa26b5740c7538aa1df1f97dcab12c3a743c2048f6c9a754f66189ac0f21544399798fb780cd347c9cac0443c8d778736938e17cdd5eca8a2338d8171efd61e13c868dff862da9df4ca8c653a227e0971030aa7e6b44dc2199d1ebd9cae00c6f0a3e91bb883cc509fb297902ba5c13e5826071d92178ace51f1a0653b0445cf7ba17226401c92d7db4f67a37d1243f9094ad5f32873891ea5004a8cbfec77129d4955e344492aaee456f852001ded",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=CN, L=Shanghai, O=miHoYo Co.,Ltd., OU=OPS, CN=miHoYo Co.,Ltd.",
      "ValidFrom": "2019-04-08 00:00:00",
      "ValidTo": "2022-04-08 12:00:00"
    },
    {
      "Signature": "5cf5b22d02ceed01b53512d813f7aa4014c7a15ca08a55ed7e55ea6ac457176fd04722423658efc5ac61c5f62c52ce6ae6c80d85dab334420ea40225182672b92a4ea57e4b16f2a0e40c449ce24d9af474f0f927a6699031c244654348c74869d0fc8409f286140ac22996857f11eb8713176ed3ec6bff1d578ab17b1ea5a07ce9a27a68e5fac6b161d67263fa379163835599f81d614f0c6fa3f7bcb1152acc8d85e31417ef7e49443fb022c0f0acbe2fdbe10c86b0f4585c5a10a94bcdf3448a4652083e0a6210e9459504b78b8d4b074f500db7bbe7fb8ca27878c6c53b7663b2cfe521845a66fce04c79834ecfa8ee700586587cc29cd73ca3ad3c7e76625c87d0ed7cd5c55b1421f4be75a275d2e9e15ad020307841624d6b5e6e1b1710244ad8588775d015d762bbfd185665842561977faad49df4f35d6da031c2e19e02ac3e90c3327ee832903416d08b14cf95accee58c54a265b8bfed186a57073ed3e79a4a2f081a041c49871a8ae61b08a365d81c31c50d9cbab368ddf45076160675fec403e7d13edfdc862e10027e661296534e7af3365879b12042d8963f35be3f8ef2999743f5e40ce13c68728c8d49d75a52b573fb7a35943a61b08482c04885c19732d39b725fa0d2348f7ef0467cf28c7294c707b0d7b5b230b81965f09c8327b0a0abd0a2727e050fb3aeddb95b9b42bcc32663456b86f11d4643edc8",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Root CA",
      "ValidFrom": "2011-04-15 19:41:37",
      "ValidTo": "2021-04-15 19:51:37"
    },
    {
      "Signature": "9d257e1b334db226815c9b86ce23200f8087e588ffffb1d46a2c31ed3a17197117cda91bbc5a1639009de36c84e45a40fbde06018c37fa9bb19d247efe20a457ad5bb79ab06026ea6957215d342f1f71b0839419056b359010a07b97c7f63fe7e21141a6bd62d9f0273d381d286f3a5209f0ec7062d3624bb0e073a692c0d38e31d82fe36d171306eee403b614abf38f43a7719d21dd14ca155d9241daf90f81d199740d26c40e7f1bb5f5a0f1c677062815e9d893e55516f0bb0aab1cdb5c482766c8a38b0a1ce595daaec42e59a061dddaf36da261e98a0b6dec1218bdf755544003922b6bc251c20a48afb0d46ee0f4140a3a1be38f3dcaaf6a8d7bdcd844",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert, CN=DigiCert Timestamp Responder",
      "ValidFrom": "2014-10-22 00:00:00",
      "ValidTo": "2024-10-22 00:00:00"
    },
    {
      "Signature": "7b721d64ff88c83ac1b7e9e7a9c487bbdb9492d7905933fa2b87dea85b80253f138f9b831b7c43c4e68cdf393ec315ecb0da3b21257b24c1725db84791811346fa9c3f6a5138deb425cbf0abdfc528015479104624d1380f26a161904dbabd28e63ff1c4aa9bf6da35534fc9f23dd36cdc23edaaa04d6709f33a803d3cfb364c90e776a4ddf23abf56352fa24c65e8e0d4dad1c7c8916a2d234f373b199418d4d59c103cd5b11c19ff8fc86b9b9ef8ae9c999678d1cd9c51155b4226725a8d0a4a239240e886de22c2933ad49b68a6df297f06b93c0ebd9fc4869c82474271328609997209794b9d7169f541ff7f397764f1848dbe8b1eb27d68a3a590b10cff",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Code Signing CA,1",
      "ValidFrom": "2011-02-11 12:00:00",
      "ValidTo": "2026-02-10 12:00:00"
    },
    {
      "Signature": "46503ec9b72824a7381db65b29af52cf52e93147ab565c7bd50d0b41b3efec751f7438f2b25c61a29c95c350e482b923d1ba3a8672ad3878ac755d1717347247859456d1ebbb368477cc24a5f3041955a9e7e3e7ab62cdfb8b2d90c2c0d2b594bd5e4fb105d20e3d1aa9145ba6863162a8a833e49b39a7c4f5ce1d7876942573e42aabcf9c764bed5fc24b16e44b704c00891efcc579bc4c1257fe5fe11ebc025da8fefb07384f0dc65d91b90f6745cdd683ede7920d8db1698c4ffb59e0230fd2aaae007cee9c420ecf91d727b716ee0fc3bd7c0aa0ee2c08558522b8eb181a4dfc2a21ad49318347957771dcb11b4b4b1c109c7714c19d4f2f5a9508291026",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID CA,1",
      "ValidFrom": "2006-11-10 00:00:00",
      "ValidTo": "2021-11-10 00:00:00"
    }
  ],
  "CertificatesInfo": "",
  "Signer": [
    {
      "Issuer": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Code Signing CA,1",
      "SerialNumber": "05a7559541e0fdc678d79e3272468907"
    }
  ],
  "SignerInfo": ""
}
```

{{< /details >}}
-----



[*source*](https://github.com/magicsword-io/LOLDrivers/tree/main/yaml/50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3.yaml)

*last_updated:* 2023-05-22








{{< /column >}}
{{< /block >}}
