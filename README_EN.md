# 🎉 Welcome to the xray-plugins! 🎉

We have created a dedicated repository for various plugins to facilitate sharing and using different plugins. We will periodically push new plugins here, and we warmly welcome contributors to submit their plugins to enrich this repository together.

[中文版本](./README.md)

## 📂 Plugin File Formats

The plugins in this repository include fingerprints, POCs, and some specific runtime file lists. It is recommended to use the following tools to run these plugins:

- Fingerprints: Recommended to run with xapp
- POCs: Recommended to run with xpoc

## ⚠️ Usage Notice

Please note that the plugins in this repository have only been verified with xlint and have not been tested on actual targets. Therefore, the content of these plugins may not be fully usable. We recommend verifying their effectiveness before use.

## ✔️ Plugin Quality

To ensure the quality and consistency of the plugins, we will promptly release the latest xlint in the [release](https://github.com/chaitin/xray-plugins/releases) section of this project, specifically for linting plugins. The only requirement for plugins stored in this repository is to pass the xlint check.

### Usage Guide

```sh
xlint --script xxx.yml
```

For more guidelines on plugin fixes, please refer to [Plugin Fix Guide](https://docs.xray.cool/plugins/yaml/Fix).

## 🎁 Contribution Rewards

We greatly appreciate the efforts of every plugin contributor! To express our gratitude, we will occasionally send some peripheral gifts to plugin contributors. If you are interested in contributing plugins, please feel free to submit a PR or contact the project maintainers.

## 📜 Repository Structure

- `finger/`: Stores fingerprints.
- `poc/`: Stores POCs.
- `group/`: Stores some specific runtime file lists.

## 🛠️ How to Contribute

1. **Fork** this repository.
2. **Clone** it locally for modification.
3. **Commit** your changes and push them to your Fork repository.
4. Submit a **Pull Request**, and we will review and merge your contribution as soon as possible.

## 📞 Contact Us

If you have any questions or suggestions during use, please feel free to provide feedback through the [xray repository](https://github.com/chaitin/xray/issues) page.

Thank you for your participation and support! We look forward to working with you to build a powerful and practical plugin library.

---

## 📢 Disclaimer

All content in this repository is for learning and research purposes only. Please do not use it for illegal purposes. We are not responsible for any direct or indirect damages caused by using these plugins.

## 📄 License

This project is released under the [GPL License 3.0](./LICENSE). You are free to use, modify, and distribute this project, but please retain the original author information.