# Chinese Self-Study Tutor

这是一个面向英语或德语母语汉语初学者的自适应 Codex Skill。它可以批改作业、提供范文、讲解语法和词汇、制作汉字课程、进行随堂测试、总结反复出现的问题，并通过语音功能开展口语训练。

## 安装与调用

本源码包会同步安装到 `C:\Users\liangjiayin\.codex\skills\chinese-self-study-tutor`。Codex 可以在汉语学习请求中自动选择它，也可以使用 `$chinese-self-study-tutor` 显式调用。

示例：

- `$chinese-self-study-tutor normal：批改这篇日记。`
- `$chinese-self-study-tutor detailed：用德语讲解“把”字句。`
- `$chinese-self-study-tutor full：用天、地、人制作一套课程和测试。`
- `$chinese-self-study-tutor 通过语音和我练习在餐馆点菜。`

## 反馈深度

可以指定 `quickest`、`simple`、`normal`、`detailed` 或 `full`，也可以让老师自行判断。这些档位是灵活的深度建议，不是固定模板。`normal` 及以上会自动归档；存在输入文件或明确要求输出文件时，默认至少使用 `normal`。

除非明确要求不要拼音，否则所有档位都会为教学中的中文提供带声调拼音。老师会悲观估计学习者当前的中文水平：存在多个可能档位时，默认按较低档位讲解，只有在反复出现明确证据或用户主动要求时才提高难度。

`normal` 档位的作文和批改会逐句给出订正后的中文、对应拼音、中文语序拆解、直译、自然翻译、重点讲解和简短练习。例如：

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
I / these two days / all / work from home
Natural English: I have been working from home these past two days.
```

## 归档

达到归档深度的内容会以自包含 HTML 保存到当前工作区的 `archive` 目录，并分入 `homework`、`tests`、`knowledge`、`speaking` 和 `reviews`。原始输入文件不会被改动。文件名采用 `YYYYMMDD 标题.html` 和 `YYYYMMDD [状态] 标题.html`；同名时增加数字后缀，不覆盖旧文件。

讲解语言默认是英语；用户要求或明显偏好德语时改用德语。中文默认采用普通话和简体字，也可按要求调整。
