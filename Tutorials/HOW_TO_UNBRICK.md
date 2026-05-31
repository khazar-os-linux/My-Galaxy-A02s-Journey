# How to unbrick the Galaxy A02s 

Quick guide to unbrick **Samsung Galaxy A02s (MSM8953)** using `edl` tool on Linux.

### Firstly connect your phone to PC and run `lsusb` command. Look for 
`05c6:9008 Qualcomm, Inc. Gobi Wireless Modem (QDL mode)`
### or similar output. If you see it download the [Firmware_Files_for_EDL](https://www.mediafire.com/file/8gmqdfyfsar508p/HardBrick+Fix.7z/file) and just run this command inside the directory containing the firmware files: 

```
sudo edl xml=rawprogram0.xml --loader=prog-emmc-firehose-8953-ddr.mbn
```

_Note: No `patch0.xml` is required. The tool will parse and flash the partition layout directly without errors._
