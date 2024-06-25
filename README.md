## 🎉 欢迎来到插件存储库！🎉

我们为各类插件创建了一个专门的存储库，旨在方便大家共享和使用各种插件。

这里主要收录的是开源的、转化成 xray格式的脚本，以供大家使用。

我们会不定期地往这里推送一些新的插件，同时也希望大家能积极踊跃的优化或者提交插件，共同丰富这个仓库。

[English Version of README](./README_EN.md)

## 📂 插件文件格式

本仓库中的插件包括指纹、POC 以及一些指定运行的文件列表。推荐使用以下工具来运行这些插件：

- 指纹：推荐使用 xapp 运行
- POC：推荐使用 xpoc 运行
- Group List：其中存放着一些梳理过的指定运行的文件列表，推荐使用xapp、xpoc -g 运行。

## ⚠️ 使用须知

请注意，本仓库中的插件仅经过 xlint 验证，未经过实际靶站的验证，因此这些插件的内容可能并不一定完全可用。我们建议在使用之前自行验证其有效性。

## ✔️ 插件质量

为了确保插件的质量和一致性，我们会在本项目的 [release](https://github.com/chaitin/xray-plugins/releases) 中及时发布最新的 XLint，专门用于 lint 插件。存放在本仓库的插件唯一要求就是通过 CI 中的 lint 检查。

### 使用指南

```sh
xlint -f xxx.yml
xlint -f "./finger/*"
xlint -f "./finger/*" -f "./poc/*"
```

## 📜 收录标准

本仓库收录的内容包括：

1. 插件优化：对现有插件进行优化，或者将不同来源但检测同一产品或漏洞的插件进行优化合并。
2. Group List：提交自用的好用的 [Group List](./group/README.md)。
3. 新的插件。

更多关于插件修复的指南，请参考 [插件修复指南](https://docs.xray.cool/plugins/yaml/Fix)。

###  仓库结构

- `finger/`：存放指纹，分为 `web` 和 `service` 两个文件夹。
    - `manual/`：存放手工编写的指纹。
      - `web/`：存放 Web 指纹。
      - `service/`：存放服务指纹。
    - `xxx/`：存放xxx来源的指纹。
    - ...
- `poc/`：存放 POC，按不同来源分类。
    - `manual/`：存放手工编写的poc。
    - `xxx/`：存放xxx来源的poc。
    - ...
- `group/`：存放一些指定运行的文件列表。

> 注意：在提交指纹或 POC 时，应明确具体的来源。如果是自己编写的，可以将其存放到manual文件夹中，如果是指纹，请确保其中包含cpe信息。
> 
> 如果某个插件被优化合并了，应将其从原来源的文件夹中移除，并合并到 `finger|poc/manual/web|service` 文件夹中，表示该插件经过人工确认。

提交时请确认仓库中没有同产品或漏洞的插件，避免重复提交。

## 🛠️ 如何贡献

1. **Fork** 本仓库。
2. **Clone** 到本地进行修改。
3. **Commit** 你的更改，并推送到你的 Fork 仓库。
4. 提交 **Pull Request**，我们会尽快审核并合并你的贡献。

### 贡献奖励

> **如果您希望通过提交或者优化指纹获取奖励，请确保您提交或者优化的指纹中包含cpe信息**

#### 积分发放：

|  分类  |  积分  |  说明  |
| --- | --- | --- |
|  GroupList提交  |  20-500/个  |  视GroupList的时效性、完整度、可利用度、价值高低等方面综合评定，给予20-500不等的积分奖励  |
|  新插件提交  |  20/个  |  提交符合插件收录标准且包含准确cpe信息的新插件，给予20积分奖励  |
|  插件优化  |  5/个  |  对现有插件进行优化，或者将不同来源但检测同一产品或漏洞的插件进行优化合并，给予5积分奖励  |

#### 奖励兑换：

每季度开放一次奖励兑换窗口

所有本季度积分在500以上的用户均可以进入排名，不同排名奖励如下：

|  名次  |  荣誉证书  |  xray高级版  |  周边礼品  |  惊喜奖品  |   |
| --- | --- | --- | --- | --- | --- |
|  Top1  |  实体荣誉证书  |  xray高级版（90天）  |  xray社区定制周边（5选3）  |  京东卡100元  |  奖励不定时更新  |
|  Top2-5  |  电子荣誉证书  |  xray高级版（60天）  |  xray社区定制周边（2选5）  |  京东卡50元  |
|  Top6-10  |  电子荣誉证书  |  xray高级版（30天）  |  xray社区定制周边（1选5）  |  /  |
|  Top11-20  |  电子荣誉证书  |  xray高级版（15天）  |  xray社区定制周边指定1款  |  /  |
|  Top21-  |  电子荣誉证书  |  xray高级版（7天）  |  /  |  /  |

兑换方式：

成功提交后添加微信群，进群验证github用户名；每个季度结算并公开排名，用户可在社群提示的兑换时间，联系工作人员进行奖励兑换。


## 📞 联系我们

如果你在使用过程中有任何问题或建议，欢迎通过 [xray 仓库](https://github.com/chaitin/xray/issues) 页面进行反馈，或通过[帮助页面](https://docs.xray.cool/help/index)添加微信公众号，加入 xray 社区交流群。

感谢你的参与和支持！我们期待与你共同打造一个强大且实用的插件库。

---

## 📢 声明

本仓库的所有内容仅供学习和研究使用，请勿将其用于非法用途。对因使用这些插件导致的任何直接或间接损害，我们概不负责。

## 📄 开源协议

本项目基于 [GPL License 3.0](./LICENSE) 开源协议进行发布。你可以自由地使用、修改和分发本项目，但请保留原作者信息。