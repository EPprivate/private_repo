# Article Analysis: Multiple Selections

Looking through the JetBrains IntelliJ IDEA documentation library, I've come across [this](https://www.jetbrains.com/help/idea/pro-tips.html#multiple-selections) short article about the **Multiple Selections** feature.

At first sight, the descriptions are looking clear and straightforward. However, when you start reproducing them in IntelliJ IDEA, some procedures described in the instruction may start to seem confusing. In the following sections, I will try to provide a reasoning for each part that I found troublesome.

## Issue 1: Unclear Use Case

There is no use case provided for this feature. The user is left unaware of the situation where he or she can apply the acquired knowledge. Can you use this feature as  a more controllable (in a way that you can select and edit a specific amount of fragments, as opposed to editing all corresponding occurances) alternative to [rename refactorings](https://www.jetbrains.com/help/idea/rename-refactorings.html) functionality? Or is it intended for something completely different?

## Issue 2: Vague Description of the Alt+Shift+J Key Combination

The description of the `Alt+Shift+J` key combination in the following line is inaccurate:

| You can press `Alt+J` again to go forward, or `Alt+Shift+J` to go back... |
|---|

The wording in this sentence may lead someone to a conclusion, that it is possible to select similar fragments both downwards and upwards to the selection starting point, which is not the case. Pressing the `Alt+Shift+J` key combination does not allow you to select the matching fragment above the first selected element, it just  cancels the previous selection.

![issue_2](https://github.com/EPprivate/private_repo/blob/main/images/issue_2.gif?raw=true)

## Issue 3: Inaccurate Description of the Clone Caret Feature

The _hot tip_ about the caret cloning may be hard to reproduce because of the inaccurate description. The instruction contains the following line:

| _Hot tip_: One more way to clone caret is to press `Ctrl` twice, and then move the caret up or down with arrows or with the mouse. |
|---|

However, if you press the `Ctrl` button twice, and then try to move the caret, you won't be able to do so because the **Run Anything** dialog is opened:

![issue_3](https://github.com/EPprivate/private_repo/blob/main/images/issue_3.gif?raw=true)

If you want to clone the caret, you have to **hold** the `Ctrl` button after you pressed it for the second time, and then move the caret up or down with arrows (I was not able to move it with the mouse for some reason).

Moreover, I'm not sure if this tip is relevant at all. In my opinion, this is a rather situational feature that can be used in a limited number of cases. The caret is cloned at a specific position, which means that this feature can only be used for the fragments that are located at the same indentation level. All this makes the tip irrelevant because the method described in the article (`Alt+J`) is much more convenient to use.

## Issue 4: Missing Feature Description

There is one more usage of the `Alt+J` key combination that is not described in the article. If you want to select all matching fragments in the file, you can simply hold the `Alt+J` key combination, instead of pressing it multiple times, as it is suggested in the instruction.

![issue_4](https://github.com/EPprivate/private_repo/blob/main/images/issue_4.gif?raw=true)

## Additional Comment: "A Relatively New Feature"

Not an issue, rather a comment. There is a following line in the article:

| Multiple selection is a relatively new, very powerful editor feature... |
|---|

However, it seems that this feature has been around for a while. Its description exists at the very least in the `2020.1` version of the documentation.

![new_feature](https://github.com/EPprivate/private_repo/blob/main/images/new_feature.png?raw=true)

Probably, it is better to avoid such phrases in documentation, especially when you need to maintain so much of it, because descriptions like this get forgotten very fast, and are rarely changed as a result.
