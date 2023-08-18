# Anytype 非官方中文教程

本仓库由社区成员共同撰写、整理、维护，欢迎大家积极反馈，共同参与 Anytype 社区的建设与贡献

Anytype 中文社区（非官方）：

**QQ群**： xxxx

**QQ频道**： xxxx

## 项目介绍

本项目为非官方中文教程的整理集合，旨在帮助 Anytype 中文用户更好地了解和使用 Anytype。

## 目录

- [Anytype 非官方中文教程](#anytype-非官方中文教程)
  - [项目介绍](#项目介绍)
  - [目录](#目录)
  - [安装和配置](#安装和配置)
  - [界面和功能介绍](#界面和功能介绍)
  - [数据类型和操作](#数据类型和操作)
  - [高级功能和扩展](#高级功能和扩展)
  - [常见问题和解决方案](#常见问题和解决方案)
  - [贡献指南](#贡献指南)
    - [我不是一名开发者](#我不是一名开发者)
    - [我是一名开发者](#我是一名开发者)
      - [项目结构](#项目结构)
      - [开发规范](#开发规范)
        - [命名形式](#命名形式)
        - [代码规范](#代码规范)
      - [文档编写](#文档编写)
      - [文档翻译](#文档翻译)

## 安装和配置

Anytype 的安装和配置方法

## 界面和功能介绍

Anytype 的界面和基本功能

## 数据类型和操作

Anytype 中的数据类型和操作

## 高级功能和扩展

Anytype 的高级功能和扩展

## 常见问题和解决方案

Anytype 的常见问题和解决方案

## 贡献指南

> 本项目 markdown 采用 markdownlint 规范

### 我不是一名开发者

请将已经编写好的 Markdown 文档发送至本仓库的开发人员，并在发送时 @ QQ群管理员以便及时更新。

### 我是一名开发者

1. Fork 本仓库
2. 新建 feat/xxx 分支
3. 提交代码
4. 新建 Pull Request

注意：请使用git rebase -i合并 commit，确保每次 pr 只有一次 commit。操作流程请参考[相关文档](https://zhuanlan.zhihu.com/p/429214913)

#### 项目结构

```bash
anytype-tutorials-cn/
├── assets/
│   ├── app.css           # css文件
│   ├── index.html        # 首页
├── config/               # 配置文件
│   ├── zh.yml            # 中文配置
├── docs/                 # 文档
│   ├── zh/               # 中文文档
├── scripts/              # 脚本文件
└── theme_override/        # 主题文件
```

#### 开发规范

##### 命名形式

1. camelCase: 驼峰式
2. kebab-case: 短横线连接式
3. PascalCase: 帕斯卡命名式
4. Snake: 下划线连接式

文件夹及文件命名采用`kebab-case`

##### 代码规范

1. 变量命名做到见名知义，方法命名使用动词或动宾结构
2. 使用markdownlint规范编写markdown文档
3. 使用prettier格式化代码
4. 提交前请运行 `bash ./scripts/build` 检查, 开发均在 `bash ./scripts/serve` 启动的服务上进行.确认无问题后提交。
5. `git commit`信息请尽量参照[相关规范](https://www.conventionalcommits.org/zh-hans/v1.0.0/)
6. 其他注意事项请参考业界相关通用开发规范说明

#### 文档编写

1. 在 docs/zh/ 目录下创建一个新的子目录，并使用 kebab-case 命名法来命名该子目录中的文件。请注意，**应避免使用拼音命名法**。
2. 修改 config/zh.yml 文件，在 nav 下添加指向新文档的链接。

#### 文档翻译

1. 在 docs/ 目录下创建一个新的子目录，并使用待翻译语言的 [ISO 639-1代码](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) 代码 来命名该子目录。例如，zh 代表中文，en 代表英文。将 docs/zh 目录中的内容复制到新建的子目录中，并进行相应的翻译工作。
2. 在 config/ 目录下创建一个新的文件，并使用待翻译语言的 [ISO 639-1代码](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) 代码 来命名该文件。例如，zh.yml 代表中文，en.yml 代表英文。将 zh.yml 文件中的内容复制到新建的文件中，并修改其中的链接地址以适应新的子目录。
3. 修改 index.html 文件，在其中添加对应的语言及国旗。
