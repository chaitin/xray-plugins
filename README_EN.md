## 🎉 Welcome to the Plugin Repository! 🎉

We have created a dedicated repository for various plugins, aiming to facilitate the sharing and use of different plugins.

This repository primarily includes open-source scripts converted to the xray format for everyone to use.

We will periodically push new plugins here, and we encourage everyone to actively optimize or submit plugins to enrich this repository together.

[中文版 README](./README.md)

## 📂 Plugin File Format

The plugins in this repository include fingerprints, POCs, and some specific run file lists. We recommend using the following tools to run these plugins:

- Fingerprints: Recommended to run with xapp
- POCs: Recommended to run with xpoc
- Group List: Contains curated lists of specific run files, recommended to run with xapp or xpoc -g.

## ⚠️ Usage Notice

Please note that the plugins in this repository have only passed xlint validation and have not been tested on actual targets. Therefore, the content of these plugins may not be fully usable. We recommend verifying their effectiveness before use.

## ✔️ Plugin Quality

To ensure the quality and consistency of the plugins, we will promptly release the latest xlint in the [release](https://github.com/chaitin/xray-plugins/releases) section of this project for linting plugins. The only requirement for plugins stored in this repository is to pass the lint check in the CI.

### Usage Guide

```sh
xlint -f xxx.yml
xlint -f "./finger/*"
xlint -f "./finger/*" -f "./poc/*"
```

## 📜 Inclusion Criteria

The content included in this repository includes:

1. Plugin Optimization: Optimize existing plugins or merge plugins from different sources that detect the same product or vulnerability.
2. Group List: Submit useful personal [Group List](./group/README.md).
3. New Plugins.

For more guidelines on plugin fixes, please refer to [Plugin Fix Guide](https://docs.xray.cool/plugins/yaml/Fix).

### Repository Structure

- `finger/`: Stores fingerprints, divided into `web` and `service` folders.
    - `manual/`: Stores manually written fingerprints.
        - `web/`: Stores web fingerprints.
        - `service/`: Stores service fingerprints.
    - `xxx/`: Stores fingerprints from xxx source.
    - ...
- `poc/`: Stores POCs, categorized by different sources.
    - `manual/`: Stores manually written POCs.
    - `xxx/`: Stores POCs from xxx source.
    - ...
- `group/`: Stores curated run file lists.

> Note: When submitting fingerprints or POCs, the specific source should be clearly stated. If it is self-written, it can be stored in the manual folder. If it is a fingerprint, ensure it contains CPE information.
>
> If a plugin has been optimized and merged, it should be removed from the original source folder and merged into the `finger|poc/manual/web|service` folder, indicating that the plugin has been manually verified.

Before submission, please ensure there are no duplicate plugins for the same product or vulnerability in the repository.

## 🛠️ How to Contribute

1. **Fork** this repository.
2. **Clone** it locally to make modifications.
3. **Commit** your changes and push them to your Forked repository.
4. Submit a **Pull Request**. We will review and merge your contributions as soon as possible.

### Contribution Rewards

> **If you wish to receive rewards for submitting or optimizing fingerprints, please ensure that the fingerprints you submit or optimize include CPE information.**

#### Points Distribution:

|  Category  |  Points  |  Description  |
| --- | --- | --- |
|  GroupList Submission  |  20-500/each  |  Points awarded based on the timeliness, completeness, usability, and overall value of the GroupList, ranging from 20 to 500 points.  |
|  New Plugin Submission  |  20/each  |  Submit new plugins that meet the inclusion criteria and include accurate CPE information for 20 points.  |
|  Plugin Optimization  |  5/each  |  Optimize existing plugins or merge plugins from different sources that detect the same product or vulnerability for 5 points.  |

#### Reward Redemption:

The reward redemption window opens once per quarter.

All users with over 500 points in the current quarter can enter the ranking, with different rewards for each rank as follows:

|  Rank  |  Honor Certificate  |  xray Pro Version  |  Merchandise  |  Surprise Prize  |   |
| --- | --- | --- | --- | --- | --- |
|  Top1  |  Physical Honor Certificate  |  xray Pro Version (90 days)  |  xray Community Custom Merchandise (choose 3 out of 5)  |  100 RMB JD Card  |  Rewards updated periodically  |
|  Top2-5  |  Electronic Honor Certificate  |  xray Pro Version (60 days)  |  xray Community Custom Merchandise (choose 2 out of 5)  |  50 RMB JD Card  |
|  Top6-10  |  Electronic Honor Certificate  |  xray Pro Version (30 days)  |  xray Community Custom Merchandise (choose 1 out of 5)  |  /  |
|  Top11-20  |  Electronic Honor Certificate  |  xray Pro Version (15 days)  |  Specified xray Community Custom Merchandise  |  /  |
|  Top21-  |  Electronic Honor Certificate  |  xray Pro Version (7 days)  |  /  |  /  |

Redemption Method:

After successfully submitting, join the WeChat group and verify your GitHub username in the group; points are settled and rankings are made public each quarter. Users can contact staff for reward redemption during the specified redemption time announced in the community.

## 📞 Contact Us

If you have any questions or suggestions during use, feel free to provide feedback via the [xray repository](https://github.com/chaitin/xray/issues) page, or join the xray community discussion group through the [Help Page](https://docs.xray.cool/help/index) by adding the official WeChat account.

Thank you for your participation and support! We look forward to working with you to create a powerful and practical plugin library.

---

## 📢 Disclaimer

All content in this repository is for learning and research purposes only. Do not use it for illegal purposes. We are not responsible for any direct or indirect damage caused by the use of these plugins.

## 📄 Open Source License

This project is released under the [GPL License 3.0](./LICENSE). You are free to use, modify, and distribute this project, but please retain the original author information.