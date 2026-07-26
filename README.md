# TokenHub License 签发台 · 安装包下载

**TokenHub License Issuer** 是 TokenHub 内部使用的单机离线 License 签发工具（授权人员专用）。
不联网、不起服务器，签发私钥全程只在内存解密、签完即擦除，绝不落盘。

> 本仓库**只用于分发 macOS 安装包和版本信息**，不包含源代码。

## ⬇️ 下载最新版

👉 **[前往 Releases 下载最新版本](https://github.com/tomszhou/token-license-release/releases/latest)**

在最新 Release 的 **Assets** 区域下载 `.dmg` 文件即可。

## 💻 系统要求

- macOS 11（Big Sur）或更高版本
- **Apple 芯片（M1 / M2 / M3 …）** —— 当前安装包为 Apple Silicon (arm64) 版本，暂不支持 Intel Mac

## 📦 安装

1. 双击下载好的 `.dmg`
2. 把 **TokenHub License Issuer** 拖进 **Applications（应用程序）** 文件夹
3. 从启动台 / 应用程序里打开

安装包已经过 **Apple 公证（Notarized）**，正常双击即可打开，不会出现「无法验证开发者」的拦截。

## 🔎 获取最新版本（程序查询）

```
https://api.github.com/repos/tomszhou/token-license-release/releases/latest
```

返回 JSON 中的 `tag_name` 即最新版本（如 `v0.1.0`），`assets[].browser_download_url` 为安装包直链。

## 🔐 使用须知

- 本工具用于签发 License，**仅限授权人员使用**；签发私钥（加密 PEM）请自行安全保管，切勿随工具分发。
- 首次使用请先在工具内「生成密钥对」得到加密私钥 + 公钥，再用私钥签发 License；公钥交给验签方内置。

## 🗒 版本历史

### v0.1.0
- 首个发行版：签发凭证台（授权信息表单 + 私钥密码保护）、生成密钥对、加密私钥支持
