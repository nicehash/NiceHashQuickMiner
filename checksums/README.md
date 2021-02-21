# SHA1 & SHA256 Checksums for RELEASE files

After downloading a file, make sure the downloaded file has matching SHA1 & SHA256 hash. If you don't know how to do that, 
download and install [7z](https://www.7-zip.org/download.html). In File Explorer, right click downloaded file, then select `CRC SHA` then `*`.

![How to check SHA hash](https://github.com/nicehash/NiceHashQuickMiner/blob/main/checksums/howtohash.png?raw=true)

If the file's SHA1 or SHA256 does not match **precisely with each letter and number** then under any condition **DO NOT USE THE FILE!** Mismatching checksums means that someone has tampered with the file hence the file is not from NiceHash but someone else and you cannot trust this file.

File Name | Checksum
----------|--------------
[NiceHash_QuickMiner_v0.3.2.2_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.2_RC) | **SHA1:** F20A32ADCFA17012D7C36949C8A8CBA8B1176A96<br> **SHA256**: F4BE323F22690579DCF6160F8EC6E48D9F22F3739E4D5280838CB4CEF74A3957
[NiceHash_QuickMiner_v0.3.2.1_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.2.1_RC) | **SHA1:** 01EDCA09212394937E7A31FED6E57F5C791D3A1D<br> **SHA256**: 3267AF25B6783A9DEDF6515C144CF2C9B62A39E24CF09BED3CF4D22DEE90C877
[NiceHash_QuickMiner_v0.3.0.2.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.2) | **SHA1:** 5BE5A32C7FF1C840B522EC0B891BABD921BF8056<br> **SHA256:** 285E38F942655B0D988F2B421CCB478E8CCAF675DCCA814D8CAB301F205AA2BA


`.NHPKG` (NiceHash package) files are automatically checked by NiceHash QuickMiner after being downloaded. This means that auto-update feature of NiceHash QuickMiner takes care of security of your system. SHA256 checksum of the package is provided with the version information from [latest_version.json](https://github.com/nicehash/NiceHashQuickMiner/blob/main/update/latest_version.json).
