# FindStar 1.3.0 Windows 预览包

这是未签名的 Windows 11 x64 预览软件，内置运行库，无需另装 Python 或 Node。真实 Windows 实机和真实 API 尚未验证。

## 下载和启动
1. 在仓库首页点击 Code → Download ZIP，然后完整解压仓库 ZIP。
2. 打开 delivery/FindStar-1.3.0 文件夹。保持全部 21 个 .part 分卷、SHA256SUMS.json 和 Merge-FindStar.cmd 在同一目录，不要逐个解压分卷。
3. 双击 Merge-FindStar.cmd。脚本使用 Windows 自带 PowerShell，逐卷验证大小和 SHA256，然后拼接并校验完整 ZIP；缺卷或错误卷会停止，不覆盖已有不同文件。
4. 看到 SUCCESS 后，对生成的 FindStar-Windows-x64-v1.3.0.zip 选择“全部解压”，进入 FindStar 文件夹，双击 FindStar.exe。不要在 ZIP 预览中启动，也不要只取出 EXE。

合并脚本未在真实 Windows 执行；ZIP CRC、原软件测试和分卷重组校验已完成。Windows 可能显示发行者未知，请核对来源与校验值，不要关闭安全防护。API 为可选，默认可进行本地关键词检索。详细说明和测试报告在软件 ZIP 内。

原始 ZIP SHA256：`34f6483290380574461d438e4ea2c40d33d320ec4f94f140b29eeb8f89b86ecb`

分卷只是原 ZIP 的原始字节切分，未重新压缩、编译或修改软件。
