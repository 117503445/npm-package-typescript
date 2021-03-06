# npm-package-typescript

使用 TypeScript 编写 NPM 包

## 使用

1. 注册 [NPM 注册](https://www.npmjs.com)，记得去邮箱接收验证邮件，获取到 NPM_TOKEN。

2. 以本项目为模版，创建 Repo [generate](https://github.com/117503445/npm-package-typescript/generate)

3. 修改 package.json

- name 包名， 以 `@NPM账号/` 开头
- version 版本，改为 0.1.0，详见 [语义化版本](https://semver.org/lang/zh-CN)，后续版本更新使用 [Yarn version](https://yarnpkg.com/cli/version)
- description 项目描述
- author 作者
- license 许可证，详见 [spdx](https://spdx.org/licenses) 的 Identifier
- keywords 和项目有关的 关键词 数组

4. 去 GitHub Repo Setting 设置 secrets

settings - secrets - New xrepository secret

Name 填入 NPM_TOKEN，Value 填入 自己获取到的 NPM_TOKEN。

5. 去 GitHub Repo Setting 开启 Github Page API 文档托管

settings - Pages - Source 调整为 Branch: gh-pages, /(root)

以本项目为例， 可以在 <https://www.117503445.top/npm-package-typescript/> 查看持续集成的 API 文档。

## 命令

```sh
yarn test # 本地执行单元测试
yarn build # 编译，用于 CICD
yarn doc # 生成文档
```
