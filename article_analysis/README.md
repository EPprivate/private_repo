# Article Analysis: Multiple Selections

Looking through the JetBrains IntelliJ IDEA documentation library, I've come across [this](https://www.jetbrains.com/help/idea/pro-tips.html#multiple-selections) short article about the **Multiple Selections** feature.

At first sight, the descriptions are looking clear and straightforward. However, when you start reproducing them in IntelliJ IDEA, some procedures described in the instruction may start to seem confusing. In the following sections, I will try to provide a reasoning for each part that I found troublesome.

## Issue 1: Unclear Use Case



## Issue 2: Vague Description of the Alt+Shift+J Key Combination

The description of the `Alt+Shift+J` key combination in the following line is inaccurate:

| You can press `Alt+J` again to go forward, or `Alt+Shift+J` to go back... |
|---|

The wording in this sentence may lead someone to a conclusion, that it is possible to select similar fragments both downwards and upwards to the selection starting point, which is not the case. Pressing the `Alt+Shift+J` key combination does not allow you to select the matching fragment above the first selected element, it just  cancels the previous selection.

## Issue 3: Inaccurate Description of the Clone Caret Feature

The _hot tip_ about the caret cloning may be hard to reproduce because of the inaccurate description. The instruction contains the following line:

| _Hot tip_: One more way to clone caret is to press `Ctrl` twice, and then move the caret up or down with arrows or with the mouse. |
|---|

However, if you press the `Ctrl` button twice, and then try to move the caret, you won't be able to do so because the **Run Anything** dialog is opened:

![issue_2](https://github.com/EPprivate/private_repo/blob/main/images/issue_2.gif?raw=true)



## Issue 4: Missing Feature Description

The last issue I would like to discuss, is the absense of another `Alt+J` key combination use case. If you want to select all matching fragments in the file, you can simply hold the `Alt+J` key combination, instead of pressing it multiple times, as it is suggested in the instruction.
