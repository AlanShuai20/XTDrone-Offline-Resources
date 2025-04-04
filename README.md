# XTDrone-Offline-Resources

Backup of XTDrone's required data/files for easy local setup.

XTDrone 安装所需的 GeographicLib 数据集和文档归档，用于离线快速配置。所有文件均为原始版本。

```bash
  mkdir -p GeographicLib
  tar -xjvf egm96-5.tar.bz2 -C GeographicLib/ && unzip egm96.zip -d GeographicLib/ && unzip emm2015.zip -d GeographicLib/
  sudo rm -rf /usr/share/GeographicLib
  sudo mv GeographicLib/ /usr/share/
```

## Source  
- [XTDrone Official GitHub](https://github.com/robin-shaun/XTDrone)
- [仿真平台基础配置（对应PX4 1.13版）](https://www.yuque.com/xtdrone/manual_cn/basic_config_13)
- GeographicLib [geoids egm96-5](https://sourceforge.net/projects/geographiclib/files/geoids-distrib/egm96-5.tar.bz2/download)
- GeographicLib [gravity egm96](https://sourceforge.net/projects/geographiclib/files/gravity-distrib/egm96.zip/download)
- GeographicLib [magnetic emm2015](https://sourceforge.net/projects/geographiclib/files/magnetic-distrib/emm2015.zip/download)
