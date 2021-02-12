# SHA1 & SHA256 Checksums for RELEASE files

After downloading a file, make sure the downloaded file has matching SHA1 & SHA256 hash. If you don't know how to do that, 
download and install [7z](https://www.7-zip.org/download.html). In File Explorer, right click downloaded file, then select `CRC SHA` then `*`.

![How to check SHA hash](https://github.com/nicehash/NiceHashQuickMiner/blob/main/checksums/howtohash.png?raw=true)

If the file's SHA1 or SHA256 does not match **precisely with each letter and number** then under any condition **DO NOT USE THE FILE!** Mismatching checksums means that someone has tampered with the file hence the file is not from NiceHash but someone else and you cannot trust this file.

File Name | Checksum
----------|--------------
[NiceHash_QuickMiner_v0.3.0.6_RC.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.6) | **SHA1:** A1D7BBBC115EF347DA788F8614011A277AA2415D<br> **SHA256**: 2A2C89B81C527316FAB41285A68AB1A14AA874E439996AD8C4CA91C2629B7C10
package_update_0.3.0.6_RC.nhpkg | **SHA1:** 9D8AFE36CA65727CB5F4E20C103400A864B1A9FB<br> **SHA256:** C3D25EA33A3728750821D0C32AF045ADF7010DB9F7E65DB7A11BF939BA5CB808
[NiceHash_QuickMiner_v0.3.0.2.zip](https://github.com/nicehash/NiceHashQuickMiner/releases/tag/v0.3.0.2) | **SHA1:** 5BE5A32C7FF1C840B522EC0B891BABD921BF8056<br> **SHA256:** 285E38F942655B0D988F2B421CCB478E8CCAF675DCCA814D8CAB301F205AA2BA
package_update_0.3.0.2.nhpkg<br>package_update_0.3.0.2_RC.nhpkg | **SHA1:** 5A06C7CC736955827E8B386110C82418F00DA129<br> **SHA256:** 145D16C4E0C2F3411D99A781594D5AF130A131679625C3C4E0ECC6E8A683C840

`.NHPKG` (NiceHash package) files are automatically checked by NiceHash QuickMiner after being downloaded. This means that auto-update feature of NiceHash QuickMiner takes care of security of your system. SHA256 checksum of the package is provided with the version information from [latest_version.json](https://github.com/nicehash/NiceHashQuickMiner/blob/main/update/latest_version.json).
