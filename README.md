### M3u8-dl

![alt text](https://img.shields.io/pypi/v/m3u8_dl.svg)
![alt text](https://img.shields.io/travis/kedpter/m3u8_dl.svg)
![alt text](https://readthedocs.org/projects/m3u8_dl/badge/?version=latest)

M3u8-dl is a simple command-line util which downloads m3u8 file.


### Install

```bash
pip install m3u8-dl
```

### Usage

Get the HLS Request infomation from web browser with `Developer Tools`.
Such As `Request URL` and `Referer`.

```bash
# HLS_URL -> Request URL
# OUTPUT -> such as example.mp4
m3u8-dl HLS_URL OUTPUT
# code below may not work since the website server may reject an out-of-date request
m3u8-dl https://proxy-038.dc3.dailymotion.com/sec\(4pkX4jyJ09RyW9jaEyekktbBu55uix9cMXQu-o5e13EelVKd1csb9zYSD66hQl7PlA_V5ntIHivm_tuQqkANmQj8DbX33OMJ5Db-9n67_SQ\)/video/795/864/249468597_mp4_h264_aac.m3u8 -u https://proxy-038.dc3.dailymotion.com/sec\(4pkX4jyJ09RyW9jaEyekktbBu55uix9cMXQu-o5e13EelVKd1csb9zYSD66hQl7PlA_V5ntIHivm_tuQqkANmQj8DbX33OMJ5Db-9n67_SQ\)/video/795/864/ -H "Referer: https://www.dailymotion.com/video/x44iz79" -H "Origin: https://izhiqun.com" -H "Sec-Fetch-Site: cross-site" -H "Sec-Fetch-Mode: cors" -H "Sec-Fetch-Dest: empty"
```
