# hysAnalyser 

  MPEG-TS analysis，仅支持中文

## 功能概述

  hysAnalyser是一款 MPEG-TS 数据分析和转换工具 ( Github：https://github.com/zymill/hysAnalyser )

  * 1）MPEG-TS离线文件分析（PSI/SI，时间戳、码率、音视频同步，PES列表，RTP封装包列表等）

  * 2）HLS实时流接入（M3u8列表，分片缓存等分析）

  * 3）除主流的MP1/MP2/MP3/AAC/AC3/EAC3, MPEG-1/2/4，H.264/AVC、H.265/HEVC外，工具扩展支持了 H.266/VVC, AVS2, AVS3, Audio Vivid等编码格式 

  * 4）逐包分析：支持PAT/PMT/SDT/NIT/BAT/EIT/CAT/RST/TDT/TOT/DIT/SIT数据表解析；

  * 5）支持分析结果数据的导出，包括PCR，时间戳，码率，时间间距等内容

  * 6）ES导出和分析：支持按PES格式 或 ES格式导出数据；支持输出 H.264/HEVC/VVC/AVS3 Nal unit/GOP/Picture List, 也结合 flvAnalyser 分析ES

  * 7）流转换功能：从多节目流按需配置参数提取节目流, 单节目TS转存MP4/MKV;

  * 8）高级功能：流编辑修改PID，修改时间戳，修改界面名称，删除指定PID数据；

  * 9）定制化功能：非 MPEG-TS/DVB 标准数据支持;

  ES 分析功能，如果朋友们也可以通过 flvAnalyser 做 ES 分析。

（提示：hysAnalyser 部分功能需软件授权后才能使用，授权方法和费用请参考最后说明）


## 图示

### 基本信息

<center class="half">
    <img src="image/result_main.png" width="1280"/>
</center>

### 逐包分析

* 全量包

<center class="half">
    <img src="image/pkt_001.png" width="1280"/>
</center>

* PSI/SI过滤

<center class="half">
    <img src="image/pkt_002.png" width="1280"/>
</center>

* 时间戳过滤

<center class="half">
    <img src="image/pkt_003.png" width="1280"/>
</center>

* 右键菜单：PID过滤和快速定位

<center class="half">
    <img src="image/pkt_004.png" width="1280"/>
</center>

### 时间戳曲线

<center class="half">
    <img src="image/timestamp_diff.png" width="1280"/>
</center>


### ES流导出

<center class="half">
    <img src="image/pes_export.png" width="1280"/>
</center>

### ES数据分析

<center class="half">
    <img src="image/es_nalu.png" width="1280"/>
</center>

### ts流编辑

<center class="half">
    <img src="image/edit.png" width="1280"/>
</center>

### 节目提取和转换

<center class="half">
    <img src="image/trc.png" width="1280"/>
</center>


## 说明

  * 1）flvAnalyser 全免费 （除了flv分析外，还具备H264/H265/H266/AVS3等ES数据的分析和预览）

  * 2）hysAnalyser 大部分功能可免费使用。部分功能不免费，需要授权才能使用，需要的朋友可以参考文章结尾的授权说明！（微信：wybase）

  flvAnalyser综述 (Chinese): [https://cloud.tencent.com/developer/article/2344723]
  
  hysAnalyser综述 (Chinese): [https://cloud.tencent.com/developer/article/2517652]

  (知乎发布地址)[https://zhuanlan.zhihu.com/p/1902174484636631934]


## 功能详细说明 

  * TS流分析专栏 (腾讯云): [https://cloud.tencent.com/developer/column/105278]
  
  * hysAnalyser从MPEG-TS导出ES功能说明 (Chinese): [https://cloud.tencent.com/developer/article/2521046]
  
  * hysAnalyser特色的TS流编辑、剪辑和转存MP4功能说明 (Chinese): [https://zhuanlan.zhihu.com/p/1909374534462706463]
  
  * hysAnalyser逐包分析MPEG-TS的功能说明(Chinese)  [https://zhuanlan.zhihu.com/p/1912444921148839675]

  * hysAnalyser分析非标准数据的功能说明(Chinese)  [https://zhuanlan.zhihu.com/p/1919683425092233142]

## 授权联系和费用介绍

  * 知乎 (Chinese)：[https://www.zhihu.com/people/zymill]

  * 微信： wybase

  * Email: hybase@qq.com

  * 授权费用：**35 元(RMB) / 单台机器**   (永久授权，享有后续版本升级的所有新功能)

  * 授权方法

  1.入口
  
<center class="half">
    <img src="image/auth_001.png" width="480"/>
</center>
  
  2.采集机器码

<center class="half">
    <img src="image/auth_002.png" width="480"/>
</center>
  
  3.注册

<center class="half">
    <img src="image/auth_003.png" width="480"/>
</center>

## 支持和赞赏

 * 如果您愿意支持本软件的长期发展，可以通过微信赞赏。谢谢！（若赞赏额超出授权注册费用，请告知作者，以便作者及时提供授权码）

<center class="half">
    <img src="image/zs.jpg" width="480"/>
</center>

## Links

1. [MPEG-1/2/4](https://mpeg.chiariglione.org/)
2. [ITU官方](https://www.itu.int/rec/T-REC-H/en)
3. [AVS工作组](https://www.avs.org.cn/)
4. [ETSI](https://www.etsi.org/deliver/)

