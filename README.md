# NiceHash QuickMiner

Please use [Wiki](https://github.com/nicehash/NiceHashQuickMiner/wiki) (still work in progress but contains **most** of information you are after).

Why you should use NiceHash QuickMiner over NiceHash Miner? Read [here](https://github.com/nicehash/NiceHashQuickMiner/wiki/Why-NiceHash-QuickMiner).

**URGENT NOTICE! NiceHash QuickMiner is currently in BETA testing. Anyone can participate. Please, submit bugs [here](https://github.com/nicehash/NiceHashQuickMiner/issues).**

Supported hardware:
* NVIDIA GeForce GTX 1000 series with min. 6 GB of GDDRAM,
* NVIDIA GeForce RTX 2000 series with min. 6 GB of GDDRAM,
* NVIDIA GeForce RTX 3000 series with min. 6 GB of GDDRAM,
* Intel CPUs with AVX2,
* AMD CPUs with AVX2.

NiceHash QuickMiner contains latest version of [Excavator](https://github.com/nicehash/excavator) bundled with:
* watchdog (NiceHashQuickMiner.exe),
* autostart service (nhqmservice.exe),
* OCTune and
* (optional) XMRig CPU Miner (xmrig.exe).

# Download, installation, how to run, uninstallation

You can find these information in [Wiki](https://github.com/nicehash/NiceHashQuickMiner/wiki).

# FAQ

Available [here](https://github.com/nicehash/NiceHashQuickMiner/wiki/FAQ).

# Troubleshooting

Available [here](https://github.com/nicehash/NiceHashQuickMiner/wiki/Troubleshooting).

# Tips & Tricks

Available [here](https://github.com/nicehash/NiceHashQuickMiner/wiki/Tips-&-tricks).

**Larger rigs - risers and BIOS settings**

When you are running cards over risers, this adds extra instability factor to your configuration. You need to make sure your risers (comm link between CPU and GPU) are max stable. To achieve this, you need to set PCI Generation to 1 in BIOS (or at least 2). Having higher Generation introduce more instability because communication between CPU and GPU is faster and there are more chances for something to go wrong. There is no speed penalty when running Gen1 - your cards will hash at the same speed.

If one of your cards crashes during mining and you see device `ERROR` it most likely means riser instability. This is especially true, if it happens when your card is not overclocked. In this case replace riser, cable and set PCIE gen1 in BIOS.
