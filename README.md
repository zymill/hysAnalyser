# hysAnalyser

MPEG-TS Analyser, supports both Chinese and English (Support Both Chinese and English since **v1.4.000**)

<center class="half">
    <img src="image/eng_ver.png" width="804"/>
</center>

## Feature Overview

hysAnalyser is a professional MPEG-TS data analysis and conversion tool (GitHub: https://github.com/zymill/hysAnalyser). The feature list is as follows:

* 1) MPEG-TS file analysis (PSI/SI, timestamps, bitrate, audio/video synchronization, PES list, audio/video formats, RTP encapsulated packet list, etc.)

* 2) HLS live stream access (M3U8 playlist, segment caching, download bitrate)

* 3) UDP/SRT live stream monitoring (real-time bitrate curve, PCR curve, TR 101290 statistics, PSI/SI, audio/video details)

* 4) Video Play Support: Audio/Video Codec List
  - Audio Codec: MP1/MP2/MP3/AAC/AC3/EAC3/**Audio Vivid(AV3A)**/**DRA**
  - Video Codec: **AVS1/AVS+/AVS2/AVS3**, MPEG-1/2/4, H.264/AVC, H.265/HEVC, **H.266/VVC**

* 5) Packet-by-packet analysis
  - Single TS packet: trace PCR, continuity counter, encryption, adaptation field and other information
  - Single Section packet: supports parsing of PAT/PMT/SDT/NIT/BAT/EIT/CAT/RST/TDT/TOT/DIT/SIT tables, with PID filtering and quick positioning;
  - Single PES packet: trace key information such as audio/video DTS, PTS, and header attributes

* 6) ES analysis and export: supports exporting data in PES format or ES format; supports outputting H.264/HEVC/VVC/AVS1/AVS+/AVS2/AVS3 Nalunit/GOP/Picture List with frame-by-frame preview

* 7) Stream broadcasting: broadcast TS via UDP or RTP (over UDP) according to the PCR period; can be used as a live source, with modes for test verification such as 1%/2% acceleration and 1%/2% deceleration

* 8) Stream conversion: extract a program stream from a multi-program stream by configuring parameters as needed; remux a single-program TS to MP4/MKV;

* 9) Export of analysis result data, including PCR, timestamps, bitrate, time intervals, etc.;

* 10) Advanced features: stream editing to modify PID and timestamps, modify interface names, delete data of a specified PID, correct sync bytes, and correct PID continuity counter errors;

* 11) Customized features: support for non-MPEG-TS/DVB standard data (license required);

(Hint: Some value-added features of hysAnalyser require a software license to be activated. For licensing methods and fees, please refer to the notes at the end of this document.)

## UTF-8 Version (Unicode)

<center class="half">
    <img src="image/unicode.png" width="1280"/>
</center>

## Screenshots

### Basic Information

<center class="half">
    <img src="image/result_main.png" width="1280"/>
</center>

### Packet-by-Packet Analysis

* All packets

<center class="half">
    <img src="image/pkt_001.png" width="1280"/>
</center>

* PSI/SI filtering

<center class="half">
    <img src="image/pkt_002.png" width="1280"/>
</center>

<center class="half">
    <img src="image/pkt_006.png" width="1280"/>
</center>

* Timestamp filtering

<center class="half">
    <img src="image/pkt_003.png" width="1280"/>
</center>

* Context menu: PID filtering and quick positioning

<center class="half">
    <img src="image/pkt_004.png" width="1280"/>
</center>

* Context menu: PID filtering

<center class="half">
    <img src="image/pkt_005.png" width="1280"/>
</center>

### Video Playback

* H264/H265/H266/MPEG-2

<center class="half">
    <img src="image/play_h26x.png" width="1280"/>
</center>

* AVS+

<center class="half">
    <img src="image/play_avs1.png" width="1280"/>
</center>

* AVS2/AV3A (Audio Vivid)

<center class="half">
    <img src="image/play_avs2.png" width="1280"/>
</center>

### Timestamp Curve

<center class="half">
    <img src="image/timestamp_diff.png" width="1280"/>
</center>

### ES Stream Export

<center class="half">
    <img src="image/pes_export.png" width="1280"/>
</center>

### ES Data Analysis

<center class="half">
    <img src="image/es_nalu.png" width="1280"/>
</center>

<center class="half">
    <img src="image/es_gop.png" width="1280"/>
</center>

### TS Stream Editing

<center class="half">
    <img src="image/edit.png" width="1280"/>
</center>

### Program Extraction and Conversion

<center class="half">
    <img src="image/trc.png" width="1280"/>
</center>

### TS Stream Broadcasting

<center class="half">
    <img src="image/vss.png" width="1280"/>
</center>

### TS Real-Time Stream Analysis

<center class="half">
    <img src="image/udp_01.png" width="1280"/>
</center>
<center class="half">
    <img src="image/udp_02.png" width="1280"/>
</center>

## Notes

* 1) flvAnalyser is completely free (in addition to FLV format analysis, it also provides analysis of ES data such as H264/H265/H266/AVS1/AVS+/AVS2/AVS3 and GOP video preview)

* 2) Most features of hysAnalyser can be used for free. Some features require a license to be activated; please refer to the licensing notes at the end of this article! (WeChat: wybase)

hysAnalyser overview (Chinese): [https://cloud.tencent.com/developer/article/2517652]

flvAnalyser overview (Chinese): [https://cloud.tencent.com/developer/article/2344723]

(Zhihu post address) [https://zhuanlan.zhihu.com/p/1902174484636631934]

## Detailed Feature Documentation

* TS Stream Analysis Column (Tencent Cloud): [https://cloud.tencent.com/developer/column/105278]

* hysAnalyser — a distinctive TS stream analysis tool: [https://cloud.tencent.com/developer/article/2517652]

* hysAnalyser video format analysis capabilities: [https://cloud.tencent.com/developer/article/2609350]

* hysAnalyser UDP/SRT real-time stream analysis user guide: [https://cloud.tencent.com/developer/article/2589021]

* hysAnalyser guide to exporting ES from MPEG-TS: [https://cloud.tencent.com/developer/article/2521046]

* hysAnalyser's distinctive TS stream editing, trimming and MP4 remuxing guide: [https://zhuanlan.zhihu.com/p/1909374534462706463]

* hysAnalyser packet-by-packet MPEG-TS analysis guide: [https://zhuanlan.zhihu.com/p/1912444921148839675]

* hysAnalyser guide to analyzing non-standard data: [https://zhuanlan.zhihu.com/p/1919683425092233142]

* hysAnalyser support for parsing dual-Vivid (Audio Vivid) media information: [https://cloud.tencent.com/developer/article/2537509]

* hysAnalyser support for broadcasting files as UDP/RTP real-time streams: [https://cloud.tencent.com/developer/article/2553390]

## Licensing Contact and Fees

* Zhihu (Chinese): [https://www.zhihu.com/people/zymill]

* WeChat: wybase

* Email: hybase@qq.com

* License fees (two modes available)

  - Single-machine license: **Promotional price before January 1, 2027: 48 RMB (original price 68 RMB) / single machine** (perpetual license, includes all new features of subsequent version upgrades)

  - Two-machine license: **Promotional price before January 1, 2027: 78 RMB (original price 108 RMB) / two machines** (perpetual license, includes all new features of subsequent version upgrades)

  Note: **Existing users who licensed before January 1, 2026 can continue to enjoy the preferential price of 35 RMB per additional machine**

* Licensing method

  1. Entry

<center class="half">
    <img src="image/auth_001.png" width="480"/>
</center>

  2. Collect the machine code

<center class="half">
    <img src="image/auth_002.png" width="480"/>
</center>

  3. Register

<center class="half">
    <img src="image/auth_003.png" width="480"/>
</center>

## Support and Appreciation

* If you are willing to support the long-term development of this software, you can donate via WeChat. Thank you! (If the donation amount exceeds the license registration fee, please inform the author so that the author can provide the license code in time)

<center class="half">
    <img src="image/zs.jpg" width="480"/>
</center>

## Links

1. [TS Stream Analysis Column](https://cloud.tencent.com/developer/column/105278)
2. [MPEG-1/2/4](https://mpeg.chiariglione.org/)
3. [ITU Official](https://www.itu.int/rec/T-REC-H/en)
4. [AVS Workgroup](https://www.avs.org.cn/)
5. [ETSI](https://www.etsi.org/deliver/)
6. [hysAnalyser packet-by-packet analysis guide (with PID filtering)](https://cloud.tencent.com/developer/article/2592704)
