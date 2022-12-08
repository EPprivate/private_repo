# Article Analysis: Multiple Selections

Looking through the JetBrains IntelliJ IDEA documentation library, I've come across [this](https://www.jetbrains.com/help/idea/pro-tips.html#multiple-selections) short article about the **Multiple Selections** feature.

At first sight, the descriptions are looking clear and straight-forward. However, when you start reproducing them in IntelliJ IDEA, some procedures described in the instruction may start to seem confusing.

For example, the description of the `Alt+Shift+J` key combination contains the following line:

| "You can press `Alt+J` again to go forward, or `Alt+Shift+J` to go back...". |
|---|

The wording in this sentence may lead someone to a conclusion, that it is possible to select similar fragments both downwards and upwards of the selection starting point, which is not the case. Pressing the `Alt+Shift+J` key combination cancels the previous selection; it does not allow you to select the matching fragment above the first selected element.

The case with holding the `Alt+J` key combination, which allows you to select all matching fragments is not described at all. I think, thi should have been noticed, because otherwise, the user has to press `Alt+J` multiple times, which is not very convenient.
