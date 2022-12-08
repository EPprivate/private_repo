# Article Analysis: Multiple Selections

Looking through the JetBrains IntelliJ IDEA documentation library, I've come across [this](https://www.jetbrains.com/help/idea/pro-tips.html#multiple-selections) short article about the **Multiple Selections** feature.

At first sight, the descriptions are looking clear and straight-forward. However, when you start reproducing them in IntelliJ IDEA, some procedures described in the instruction may start to seem confusing. In the following sections, I will try to provide a reasoning for each part that I found troublesome.

## Issue 1: Possible Misinterpretation of the Instruction

The first issue I would like to discuss, is the description of the `Alt+Shift+J` key combination, specifically the the following line:

| You can press `Alt+J` again to go forward, or `Alt+Shift+J` to go back... |
|---|

The wording in this sentence may lead someone to a conclusion, that it is possible to select similar fragments both downward and upward the selection starting point, which is not the case. Pressing the `Alt+Shift+J` key combination cancels the previous selection; it does not allow you to select the matching fragment above the first selected element.

## Issue 2: Inability to Reproduce the Instruction

The second issue I wanted to point out, is the _hot tip_ about the cart cloning. The description contains the following line:

| _Hot tip_: One more way to clone caret is to press `Ctrl` twice, and then move the caret up or down with arrows or with the mouse. |
|---|

I'm not sure if the problem lies in the IntelliJ IDEA version that I use, or my keyboard shortcuts are off, but in my case, pressing the `Ctrl` button twice opens the **Run Anything** dialog, instead of cloning the caret.

## Issue 3: Missing Feature Description

The last issue I would like to discuss, is the abscense of another `Alt+J` key combination use case. If you want to select all matching fragments in the file, you can simply hold the `Alt+J` key combination, instead of pressing it multiple times, as it is suggested in the instruction.
