# SHA1 & SHA256 Checksums for RELEASE files

After downloading a file, make sure the downloaded file has matching SHA1 & SHA256 hash. If you don't know how to do that, 
download and install [7z](https://www.7-zip.org/download.html). In File Explorer, right click downloaded file, then select `CRC SHA` then `*`.

![How to check SHA hash](https://github.com/nicehash/NiceHashQuickMiner/blob/main/checksums/howtohash.png?raw=true)

If the file's SHA1 or SHA256 does not match **precisely with each letter and number** then under any condition **DO NOT USE THE FILE!** Mismatching checksums means that someone has tampered with the file hence the file is not from NiceHash but someone else and you cannot trust this file.

File Name | Checksum
----------|--------------
[NiceHashQuickMinerInstaller.exe](https://github.com/nicehash/NiceHashQuickMiner/releases/download/v0.3.2.6/NiceHashQuickMinerInstaller.exe)<br>[NiceHashQuickMinerInstaller.exe](https://github.com/nicehash/NiceHashQuickMiner/releases/download/v0.3.2.6_RC/NiceHashQuickMinerInstaller.exe) | **SHA1:** 8916BF6D926B7FE47C0FAC44E9137B09E2A1D418<br> **SHA256**: 937EEF9D69BE3EDFD7805409156411CC1609E4AE5032A8E068E9DA9098006FA6
[NiceHash_QuickMiner_v0.3.2.6.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.6)<br>[NiceHash_QuickMiner_v0.3.2.6_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.6_RC) | **SHA1:** 0EB9C540BE25424C1A42BFF3A4CAB60C4D12A975<br> **SHA256**: 2B36B8973A9A0DDDAD5E53BD6EACA5E1B376A400AB0C4A85053358A2CF2F79B6
[NiceHash_QuickMiner_v0.3.2.5_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.5_RC) | **SHA1:** 89E1E049B228672DA6D4EA1A9BA032F8E01A1C4B<br> **SHA256**: A0E8B9B7A0B985FD58C27FBA49A65447FDCB1736E238BFFB86281CCEAF88A149
[NiceHash_QuickMiner_v0.3.2.3_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.3_RC) | **SHA1:** 79040269BF929ACCDC360C4C483B5E9E58014621<br> **SHA256**: 15A03CCC5E48BC5881BE7C364B5E2AB43F11451F70EB14FFD07C81FF57F050D6
[NiceHash_QuickMiner_v0.3.0.2.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.2) | **SHA1:** 5BE5A32C7FF1C840B522EC0B891BABD921BF8056<br> **SHA256:** 285E38F942655B0D988F2B421CCB478E8CCAF675DCCA814D8CAB301F205AA2BA


`.NHPKG` (NiceHash package) files are automatically checked by NiceHash QuickMiner after being downloaded. This means that auto-update feature of NiceHash QuickMiner takes care of security of your system. SHA256 checksum of the package is provided with the version information from [latest_version.json](https://github.com/nicehash/NiceHashQuickMiner/blob/main/update/latest_version.json).
