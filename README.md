### M3u8-dl

m3u8-dl是一个命令行方式下载m3u8视频文件的小工具，改自 https://github.com/kedpter/M3u8Downloader
在M3u8Downloader基础上删减了恢复功能，并且扩展了header参数，适应性更强了


### Install

```bash
pip install m3u8-dl
```

### Usage

从浏览器的develper tools中获取*.m3u8的url信息和headers信息，编排成参数，通过程序执行就可以

例子

m3u8-dl https://proxy-038.dc3.dailymotion.com/sec\(4pkX4jyJ09RyW9jaEyekktbBu55uix9cMXQu-o5e13EelVKd1csb9zYSD66hQl7PlA_V5ntIHivm_tuQqkANmQj8DbX33OMJ5Db-9n67_SQ\)/video/795/864/249468597_mp4_h264_aac.m3u8 \
-u https://proxy-038.dc3.dailymotion.com/sec\(4pkX4jyJ09RyW9jaEyekktbBu55uix9cMXQu-o5e13EelVKd1csb9zYSD66hQl7PlA_V5ntIHivm_tuQqkANmQj8DbX33OMJ5Db-9n67_SQ\)/video/795/864/\
-H "Referer: https://www.dailymotion.com/video/x44iz79"\
-H "Origin: https://izhiqun.com"\
-H "Sec-Fetch-Site: cross-site"\
-H "Sec-Fetch-Mode: cors"
-H "Sec-Fetch-Dest: empty"

文件默认输出到当前目录下的example.mp4
