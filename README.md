# NiceHash QuickMiner
[NiceHash QuickMiner](NH_QuickMiner_v0.2.1.1_Excavator_b549.zip) (latest version: 0.2.1.1) contains latest version of Excavator bundled with:
* watchdog (NiceHashQuickMiner.exe),
* autostart service (nhqmservice.exe) and
* example command file (commands.json)

# Installation
Simply extract all files in .zip archive into any folder you want.

# How to run
Simply double click `NiceHashQuickMiner.exe` and mining process will start. You have to change mining address (to your NiceHash Mining address) - you can do this by modifying `nhqm.conf` file. Besides configuring your BTC mining address, you may want to modify following:
* serviceLocation (0 is eu, 1 is usa),
* workerName (name of your rig),
* launchCommandLine (extra command line options) and
* consoleLogLevel & fileLogLevel (logging options).

**_Please, have fileLogLevel set to 0 at all times and submit all the errors and issues you find using this software bundle. Thanks!_**

Some extra features are available in your Windows tray (notification area); right click NiceHash icon and you can add/remove autostart task or service. By enabling autostart, NiceHash QuickMiner will start with Windows automatically. NiceHash QuickMiner is bundled with CPU miner - XMRig. CPU mining is possible on CPUs that support AVX2 instruction set.

# Deinstallation
Delete all files. If you have added autostart, make sure to disable autostart before you delete all files.
Alternative way; run `NiceHashQuickMiner.exe --uninstall` and all files and folders will be purged from your PC automatically. If you also add `--keepconfig`, then config files will be kept.

# Recommendations
Also use OCTune; run `octune.html` when Excavator is running. You will get a (not-so-good-looking) interface to manage Excavator over your web browser. You can play with overclock settings. Once you are happy with your settings, just save everything by clicking on the button `Save current configuration`. Next time Excavator is started, your saved configuration will be used. You do not have to modify `commands.json` file manually anymore.

# FAQ
_1. Why is NiceHashQuickMiner started with administrator privileges?_

Administrator privileges are needed for overclocking. MSI Afterburner (which you'd not need anymore) is started with administrator privileges aswell. Since up to 20% extra performance is possible to achieve with up to 50% reduced power load, we do not believe it is smart to mine without adjusting clocks and power limits which require administrator privileges.

_2. What happens when DAG is being generated?_

Excavator would set memory overclock to 0 for the time DAG is being generated. This is done to prevent generation of corrupted DAG which causes all future shares to be invalid. Note that this feature only works if you set your overclock with Excavator and it DOES NOT work when using MSI Afterburner for overclocking. With this feature you can clock your card higher and do not need to worry about corrupted DAGs because these cannot happen anymore.

_3. Where can I see number of accepted and rejects shares?_

You can see number of accepted and rejected shares by calling [API method algorithm.list](https://github.com/nicehash/excavator/tree/master/api#algorithm-list). Note that, to the contrary of other PPLNS pools, for NiceHash, these values are not important. The reason is, because each share has a certain value that may not be the same. NiceHash does not have a fixed difficulty but rather dynamic. Higher difficulty shares have higher value. Since NiceHash has a PPS payout scheme (pay-per-share), it is very important to know the value of the share (share at twice the difficulty is worth twice as much BTC). If you chart down shares with their values, you get accepted/rejected speed. These charts are already available at NiceHash - Rig Manager. Other pools often display accepted speed on their charts as the value that the miner is reporting to the pool - and this value can be cheated-out (sending some extreme large value for example). NiceHash does not support speed reported by miner, rather it calculates accepted/rejected speed out of your shares. Thus, contrary to the other pools, these charts have very high value as they represent direct performance of your miner and your mining payouts are based directly on that.

# Troubleshooting

**_Error #102_** Excavator.exe is missing. Most likely your Antivirus (AV) or Microsoft Defender has deleted it. Make sure to add exception for following files:
* excavator.exe
* NiceHashQuickMiner.exe
* nhqmservice.exe
* xmrig.exe

**_Warning #103_** Your PC does not have enough Virtual Memory set. This can cause mining failure. Increase your Virtual Memory size to at least 6000 MB times number of GPUs your PC has. Read [here](https://www.nicehash.com/blog/post/how-to-increase-virtual-memory-on-windows) how to increase Virtual Memory size.

# Tips & Tricks

**Finding most efficient or the fastest combination of OC values for your card(s)**

Use OCTune. Look for values `Min KT` and `Avg KT`. Your goal is to get these values as low as possible. What is the meaning of these values? KT = Kernel Time. It is execution time of code running on GPU in microseconds. Min = minimal time (in previous X runs) and Avg = average time. Min can sometimes drop down to half of usual - you should ignore these values.

_1. Find your max memory clock_
First, you should find your max memory speed or determine at what memory speed you are prepared to run your GPU. Higher power limit and lower core clock can help memory stability. Therefore, set power limit to some high value (can be at 100% of your TDP - note the value needs to be in Watts!) and core clock to -600. Then increase memory clock by 25 each step and test at least several minutes. There should be no `HW err` and make sure there are at least 3 accepted shares on that card (`HW ok` increases by 3 at that speed). Once you find your max memory clock, you can go to step 2.

_2. Reduce power limit_
Now you can start reducing power limit. At some point, `Min KT` and `Avg KT` will start rising. That is a sign that you need to back off and stop reducing power limit (temporary). Now you need to increase core clock. Go to step 3.

_3. Increase core clock_
Increase core clock +25 at a time until your `Min KT` and `Avg KT` stop improving (values do not go lower anymore). Note that higher core clock can affect stability of your memory. You may have to decrease your memory clock if there are rejected shares (share above target) and value in `HW err` increases. Once you find ideal core clock, you can again try with reducing power limit.

_4. Play with settings to achieve best KT values_
You have to fiddle with core clock, memory clock and power limit until you find best KT values (lowest) and max stability (no shares above target - `HW err` stays at 0). Once you find best values, you will have the highest possible speed. You can save your OC configuration so it will be applied next time Excavator is started.

**Larger rigs - risers and BIOS settings**

When you are running cards over risers, this adds extra instability factor to your configuration. You need to make sure your risers (comm link between CPU and GPU) are max stable. To achieve this, you need to set PCI Generation to 1 in BIOS (or at least 2). Having higher Generation introduce more instability because communication between CPU and GPU is faster and there are more chances for something to go wrong. There is no speed penalty when running Gen1 - your cards will hash at the same speed.

If one of your cards crashes during mining and you see device `ERROR` it most likely means riser instability. This is especially true, if it happens when your card is not overclocked. In this case replace riser, cable and set PCIE gen1 in BIOS.
