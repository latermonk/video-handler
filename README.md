# video-hanler


*  把脚本直接放到你要转换的TS文件的目录即可
*  双击run.bat开始转换

其实就是调用ffmpeg命令：

```
.\ffmpeg -i "%%a" -f mp4 -codec copy "%%~na.mp4
```

对视频进行转换，当然如果是Linux系统就直接跑这个命令即可

```
for %%a in ("*.ts") do .\ffmpeg -i "%%a" -f mp4 -codec copy "%%~na.mp4

```
