# 捷配下单助手

<img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/klxf/eext-jiepei-helper?style=flat-square&label=Stars"><img alt="GitHub Release" src="https://img.shields.io/github/v/release/klxf/eext-jiepei-helper?style=flat-square&label=Release&color=%233fb950"><img alt="GitHub License" src="https://img.shields.io/github/license/klxf/eext-jiepei-helper?style=flat-square&label=License"><img alt="GitHub Downloads" src="https://img.shields.io/github/downloads/klxf/eext-jiepei-helper/total?style=flat-square&label=Downloads"><img alt="EasyEDA Version" src="https://img.shields.io/badge/dynamic/json?style=flat-square&url=https%3A%2F%2Fraw.githubusercontent.com%2Fklxf%2Feext-jiepei-helper%2Frefs%2Fheads%2Fmaster%2Fextension.json&query=engines.eda&label=EasyEDA&color=5588ff">

一键前往捷配下单 PCB，支持保存下单偏好，~~这很牛头人了~~

## 如何使用

### 安装扩展

参考 [嘉立创 EDA 用户指南](https://prodocs.lceda.cn/cn/api/user-guide/using-extension.html#%E5%AE%89%E8%A3%85%E6%89%A9%E5%B1%95) 安装扩展。

_使用本扩展的“检查更新”功能需要给予扩展“外部交互”权限。_

### 使用扩展

**本扩展仅在 PCB 界面激活**，菜单栏中将出现“捷配”菜单，“下单”子菜单为本扩展的主界面。

可直接在主界面选择 PCB 生产工艺参数，点击“前往下单”按钮即可前往捷配下单 PCB 页面，同时将自动导出 Berber 制板文件。

> [!IMPORTANT] > **下单前务必仔细检查所有项目是否符合预期，捷配官网可能与本扩展显示存在出入，本扩展不对工艺组合可行性进行验证，以捷配官网为准。**

**本扩展提供“工艺预设”功能**，可将常用的工艺参数保存为预设，方便下次使用：

- 【**新建预设**】在“下单”界面顶部“订单工艺预设”面板新建预设，设置工艺参数与个性化服务选项，点击底部“保存预设”按钮即可保存；
- 【**使用预设**】在“下单”界面顶部“订单工艺预设”面板选择已有的预设，将自动应用此前保存的参数与个性化选项；
- 【**删除预设**】在“下单”界面顶部“订单工艺预设”面板选择已有的预设，点击底部“删除预设”按钮即可删除。
- 【**内嵌预设**】点击“下单”界面底部的“内嵌预设”按钮即可将当前工艺参数保存到 PCB 中。若 PCB 中存在内嵌预设，扩展将自动读取。

本扩展支持自动计算：

- 【**PCB 层数**】点击“板子层数”右侧“识别”按钮后即可自动计算板子层数。**注意：EDA 仅支持绘制偶数层铜箔的 PCB，因此识别到的板子层数必然为偶数**
- 【**PCB 尺寸**】点击“板子大小”右侧的“选择板框”按钮后在画布上选择板框图元，即可自动计算板框大小。

## 即将推出的新特性

- ~~自动识别板子层数~~ ——_V1.1.0_

## 开源许可

本扩展使用 [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/) 开源许可协议。
