---
title: Markdown语法扩展
published: 2025-07-02
updated: 2025-07-02
description: '阅读更多关于Markdown语法扩展的介绍'
image: ''
tags: [Markdown]
category: 'Markdown'
draft: false 
---
## GitHub仓库卡片

你可以在页面加载时动态添加指向GitHub仓库的卡片，仓库信息来自GitHub API。

::github{repo="521xueweihan/HelloGitHub"}

使用代码创建 GitHub 存储库卡。`::github{repo="<owner>/<repo>"}`.

```markdown
::github{repo="saicaca/fuwari"}
```

## 警告

支持以下类型的警告： `note` `tip` `important` `warning` `caution`

:::note
突出显示用户应该考虑的信息，即使浏览时也是如此。
:::
:::tip
可选信息，可帮助用户更成功。
:::

:::important
用户成功所需的重要信息。
:::

:::warning
由于潜在风险，必须立即采取行动的重要内容。
:::

:::caution
某个行为可能造成的负面后果
:::

### 基本语法

```markdown
:::note
突出显示用户应该考虑的信息，即使浏览时也是如此。
:::
:::tip
可选信息，可帮助用户更成功。
:::
```

### 自定义

警告的标题可以自定义。

:::note[自定义标题]
这是一个带有自定义标题的提示。
:::

```markdown
:::note[自定义标题]
这是一个带有自定义标题的提示。
:::
```

### GitHub 语法

> [!TIP]
> [The GitHub syntax](https://github.com/orgs/community/discussions/16925)也支持.

```
> [!NOTE]
> The GitHub syntax is also supported.

> [!TIP]
> The GitHub syntax is also supported.
```