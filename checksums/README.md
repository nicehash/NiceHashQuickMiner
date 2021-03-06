# SHA1 & SHA256 Checksums for RELEASE files

After downloading a file, make sure the downloaded file has matching SHA1 & SHA256 hash. If you don't know how to do that, 
download and install [7z](https://www.7-zip.org/download.html). In File Explorer, right click downloaded file, then select `CRC SHA` then `*`.

![How to check SHA hash](https://github.com/nicehash/NiceHashQuickMiner/blob/main/checksums/howtohash.png?raw=true)

If the file's SHA1 or SHA256 does not match **precisely with each letter and number** then under any condition **DO NOT USE THE FILE!** Mismatching checksums means that someone has tampered with the file hence the file is not from NiceHash but someone else and you cannot trust this file.

File Name | Checksum
----------|--------------
[NiceHashQuickMinerInstaller.exe](https://github.com/nicehash/NiceHashQuickMiner/releases/download/v0.3.2.6/NiceHashQuickMinerInstaller.exe) | **SHA1:** 8916BF6D926B7FE47C0FAC44E9137B09E2A1D418<br> **SHA256**: 937EEF9D69BE3EDFD7805409156411CC1609E4AE5032A8E068E9DA9098006FA6
[NiceHash_QuickMiner_v0.4.0.3_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.4.0.3_RC) | **SHA1:** 325BF9CC6B942A53491B606262BEC12722078486<br> **SHA256**: C0631FCC728C97817D8A10D9D0FF1AAFCF472A608FA5A8363281E9A16D0F5C2B
[NiceHash_QuickMiner_v0.4.0.1_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.4.0.1_RC) | **SHA1:** 62D8145AA97F691217136376B34825083991EC08<br> **SHA256**: 8D3BA90BAE1609C3344B988D623B2F09A645593627E0036E6DB81CE8223276BB
[NiceHash_QuickMiner_v0.3.3.0_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.3.0_RC) | **SHA1:** CB124D0024C34020513C48DCF1CB68EEB7860F11<br> **SHA256**: F276A2DFA3A32B25271365725CC3D0A85197BA8E0D90D2AE783FB031CBFB7A18
[NiceHash_QuickMiner_v0.3.2.7_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.7_RC) | **SHA1:** AEB73A0680D388B1ED41978F60A7ADED20E79BBE<br> **SHA256**: 0E27080E622AB0D801A23A7C90989F1E922D9D21FF137426FACC381C633664DB
[NiceHash_QuickMiner_v0.3.2.6.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.6)<br>[NiceHash_QuickMiner_v0.3.2.6_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.6_RC) | **SHA1:** 0EB9C540BE25424C1A42BFF3A4CAB60C4D12A975<br> **SHA256**: 2B36B8973A9A0DDDAD5E53BD6EACA5E1B376A400AB0C4A85053358A2CF2F79B6
[NiceHash_QuickMiner_v0.3.0.2.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.2) | **SHA1:** 5BE5A32C7FF1C840B522EC0B891BABD921BF8056<br> **SHA256:** 285E38F942655B0D988F2B421CCB478E8CCAF675DCCA814D8CAB301F205AA2BA


`.NHPKG` (NiceHash package) files are automatically checked by NiceHash QuickMiner after being downloaded. This means that auto-update feature of NiceHash QuickMiner takes care of security of your system. SHA256 checksum of the package is provided with the version information from [latest_version.json](https://github.com/nicehash/NiceHashQuickMiner/blob/main/update/latest_version.json).
