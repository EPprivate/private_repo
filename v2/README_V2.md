# Tutorial: Locate, analyze, and resolve errors

Writing code is an intricate and thought-consuming process, and making errors is a part of it. It is almost inevitable that at some point a mistake will be made. Lucky for us, IntelliJ IDEA analyzes our code, inspecting both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages. The system highlights detected problems, making proofreading easier.

The whole process of fixing errors can be divided into the following steps:

1. [Locate the mistake](#locate-an-error).
2. [Analyze the detected issue](#examine-an-error).
3. [Resolve the problem](#resolve-an-error).

In this tutorial, we will go through each step

## Locate an error

You can deal with errors directly in the editor, locating and resolving problems there. However, if you need to address multiple issues, it is better to use the **Problems** tool window, since it displays a complete list of mistakes and provides a toolset for fixing them in a more centralized way. 

1. Press `Alt+6`. This key combination opens the **Problems** tool window.

2. Use the arrow keys or the mouse pointer to navigate to the desired problem.

Each listed problem has an explanation next to it and a number of the line where the error occurred.

## Examine an error

The icon near the mistake corresponds to one of the [inspection](https://www.jetbrains.com/help/idea/code-inspection.html) severity levels and depends on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

Reviewing these markings can help you to define the cause behind the problem. It is a good practice to inspect the errors to develop a strategy for a fix before proceeding to the next step.

## Resolve an error


