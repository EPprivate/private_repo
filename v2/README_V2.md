# Locate, analyze, and resolve errors

IntelliJ IDEA analyzes your code, inspecting both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages. The system highlights detected problems in the [editor](https://www.jetbrains.com/help/idea/guided-tour-around-the-user-interface.html?keymap=primary_windows) and duplicates them in the **Problems** tool window, making proofreading easier.

You can work with errors directly in the editor, locating and resolving problems there. However, if you need to address multiple issues, it is better to use the **Problems** tool window, since it displays a complete list of mistakes and provides a toolset for fixing them in a more centralized way. 

For the sake of simplicity, all procedures described in the following sections are performed in the **Problems** tool window. For information on how to locate and fix mistakes in the editor, see corresponding sections.

## Locate an error

Before fixing an error, you need to locate it first. To see the list of detected problems:

1. Press `Alt+6`. This key combination opens the **Problems** tool window.

2. Use the arrow keys or the mouse pointer to navigate to the desired problem.

Each listed problem has an explanation next to it and a number of the line where the error occurred.

## Examine an error

The icon near the mistake correspond to [inspection](https://www.jetbrains.com/help/idea/code-inspection.html) severity levels and depend on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

These markings can help you to define the cause behind the problem. Before proceeding to the next step, it is a good practice to review the errors to develop a strategy for a fix.

## Resolve an error


