
# VCEEnc  
by rigaya

**[日本語版はこちら＞＞](./Readme.ja.md)**

This software is meant to investigate performance and image quality of HW encoder (VCE) of AMD.
There are 2 types of software developed, one is command line version that runs independently, and the nother is a output plug-in of [Aviutl](http://spring-fragrance.mints.ne.jp/aviutl/).

VCEEncC.exe … Command line version supporting transcoding.  
VCEEnc.auo … Output plugin for [Aviutl](http://spring-fragrance.mints.ne.jp/aviutl/).  

## Downloads & update history
[rigayaの日記兼メモ帳＞＞](http://rigaya34589.blog135.fc2.com/blog-category-12.html)

## System Requirements
Windows 7, 8, 8.1, 10 (x86 / x64)  
Aviutl 0.99g4 or later (VCEEnc.auo)  
Hardware which supports VCE  
  AMD GPU Radeon HD 7xxx or later  
  AMD APU Trinity (2nd Gen) or later  

| VCEEnc | required graphics driver version |
|:---|:---|
| VCEEnc 3.00 or later | AMD driver 17.1.1 (16.50.2611) or later |


## Precautions for using VCEEnc
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.


## Main usable functions
### Common to VCEEnc / VCEEncC
- Encoding using VCE
   - H.264/AVC
   - HEVC (Polaris or later)
- Each encode mode of VCE
   - CQP       (fixed quantization)
   - CBR       (Constant bitrate)
   - VBR       (Variable bitrate)
- supports setting of codec profile & level, SAR, colormatrix, maxbitrate, GOP len, etc...


### VCEEncC
- Supports hw decoding
  - H.264 / AVC
  - HEVC
  - MPEG2
  - VC-1
- Supports various formats such as avs, vpy, y4m, and raw
- Supports demux/muxing using libavformat
- Supports decode using libavcodec

#### VCEEnc.auo (Aviutl plugin)
- Audio encoding
- Mux audio and chapter
- afs (Automatic field shift) support

### NVEnc source code
- MIT license.
- This program is based on samples of [AMD Media Framework](https://github.com/GPUOpen-LibrariesAndSDKs/AMF), and contains source code provided by
  AMD Media Framework.
  詳細は各ソースのヘッダ部分や、VCEEnc_license.txtをご覧ください。
- This software depends on
  [ffmpeg](https://ffmpeg.org/),
  [tinyxml2](http://www.grinninglizard.com/tinyxml2/),
  [dtl](https://github.com/cubicdaiya/dtl),
  [ttmath](http://www.ttmath.org/) &
  [Caption2Ass](https://github.com/maki-rxrz/Caption2Ass_PCR).
  For these licenses, please see the header part of the corresponding source and VCEEnc_license.txt.

### About source code
Windows ... VC build

Character code: UTF-8-BOM  
Line feed: CRLF  
Indent: blank x4  
