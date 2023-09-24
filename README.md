# prompt helper
This software is designed to facilitate the easy generation of prompts.

In the conventional method of constructing a prompt, users are required to `copy text -> paste text -> copy template prompt -> paste template prompt -> adjust the combination of the two pasted texts`. This software aims to minimize the effort involved in generating a prompt.

Ideally, I envision the prompt generation process to be as simple as `copy text -> use a hotkey (select your prompts) -> paste text`. This software aspires to realize this vision, providing a seamless and efficient user experience in prompt generation.

## What we need ?
你是一个位精通 Electron， AI， Python， CPP 的资深程序设计员。我需要设计一个 Electron 程序，所以你每次都需要给出 `html`, `css` 和 `js` 三个文件的修改。接下里是我的一些需求。我希望我们的程序能非常轻量化。

首先，我们需要一个侧边栏，侧边栏最顶上放 logo 和软件名。下面有三个 tab，一个是 `favorite`，一个是 `all`。最后一个在最底下，是 `setting`（用来设置软件的一些参数， 现在我们默认是空的）。其中 `favorite` 和 `all` 是类似文件夹的形式，可以支持多级嵌套关系和文件夹的创建。每次点击其中某个 prompt 文件便可以在右边主界面的下方进行：“预览”，“修改”（支持保存）。

关于主界面，我们需要在最上方设计一个搜索栏，搜索栏的某个位置需要能够设定不同的搜索方法（传统和向量搜索）。在搜索栏下方是一个当前剪贴板的预览，下方是之前提及的 prompt 预览窗口。每个 prompt 都有一个 `title` 和 `content`，都可以修改。在每个 prompt 的右边有一个 `copy` 按钮，点击后便可以将 `content` 复制到剪贴板中。在每个 prompt 的左边有一个 `favorite` 按钮，点击后便可以将 `prompt` 添加到 `favorite` 中。在每个 prompt 的下方有一个 `edit` 按钮，点击后便可以在主界面的下方进行修改（点击完 `edit` 之后，还会出现 `save` 和 `cancel` 按钮，点击 `save` 之后便可以保存修改，点击 `cancel` 之后便可以取消修改）。在每个 prompt 的右下角有一个 `delete` 按钮，点击后便可以将 `prompt` 删除。最后还有一个最重要的 `convert` 按钮，点击后便便可以把当前剪贴板中的内容，插入到 `prompt` 中（这要求 prompt 中有指使插入的标记，例如 `{{}}`）。

现在，请你先不用考虑 python 等后端内容，为我给出一份详细的设计代码（要求使用 bootstrap，要求扁平化，颜色绚丽的 CSS）。请你一步步的给出，并且给出你的设计思路。每次给出后，请你询问我是否满意，如果我回答满意则继续后续的代码设计。加油，相信你可以完成的！


## Reference