# SHA1 & SHA256 Checksums for RELEASE files

After downloading a file, make sure the downloaded file has matching SHA1 & SHA256 hash. If you don't know how to do that, 
download and install [7z](https://www.7-zip.org/download.html). In File Explorer, right click downloaded file, then select `CRC SHA` then `*`.

![How to check SHA hash](https://github.com/nicehash/NiceHashQuickMiner/blob/main/checksums/howtohash.png?raw=true)

If the file's SHA1 or SHA256 does not match **precisely with each letter and number** then under any condition **DO NOT USE THE FILE!** Mismatching checksums means that someone has tampered with the file hence the file is not from NiceHash but someone else and you cannot trust this file.

File Name | Checksum
----------|--------------
[NiceHash_QuickMiner_v0.3.1.2_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.1.2_RC) | **SHA1:** 23D8F009793736D780B4ECFB0B2F854094A2FD85<br> **SHA256**: 7B6BB6761B9E99F177C43924C67BF0F9C4797C2DBECD6075FE69DF68A5BD9DBB
[NiceHash_QuickMiner_v0.3.1.1_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.1.1_RC) | **SHA1:** 77C030E4A0B39D59A680ED0230E06910971213EF<br> **SHA256**: 3026BB4A3334318CD94189CAB70DFC5FE92506A99509A66A61936829C8AFE475
[NiceHash_QuickMiner_v0.3.0.7_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.7_RC) | **SHA1:** 44CACE49158C3F73EC92A5EB9F73BA67004EFB17<br> **SHA256**: 82513B33F344522FEB67929BD47B9EEB2B822191D0563D2DB92B9C006D14E822
[NiceHash_QuickMiner_v0.3.0.2.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.2) | **SHA1:** 5BE5A32C7FF1C840B522EC0B891BABD921BF8056<br> **SHA256:** 285E38F942655B0D988F2B421CCB478E8CCAF675DCCA814D8CAB301F205AA2BA


`.NHPKG` (NiceHash package) files are automatically checked by NiceHash QuickMiner after being downloaded. This means that auto-update feature of NiceHash QuickMiner takes care of security of your system. SHA256 checksum of the package is provided with the version information from [latest_version.json](https://github.com/nicehash/NiceHashQuickMiner/blob/main/update/latest_version.json).
