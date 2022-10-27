# Searching for errors

While developing an application, IntelliJ IDEA analyzes your code, highlighting the sections that require closer look. The system inspects both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages, checking syntax, spelling, and grammar. All found problems are marked in the editor and duplicated in a variety of other places, allowing you to quickly locate and resolve the issue.

## Locating errors

In IntelliJ IDEA, all error-related information is displayed:

![errors overview](https://github.com/EPprivate/private_repo/blob/main/images/errors%20overview.png?raw=true)

Markings in the editor and on the scrollbar can be used for a [brief inspection](#inspecting-errors-in-the-editor). If you want to perform a more thorough review, use the [**Problems** tool window](#inspecting-errors-in-the-problems-tool-window).

To see the statistics for detected errors, take a look at the **Inspections** widget.

![inspections widget](https://github.com/EPprivate/private_repo/blob/main/images/inspections%20widget.png?raw=true)

### Inspecting errors in the editor

Inspecting errors in the editor is convenient when there are few of them. Mistakes are highlighted as red/green wavy lines and duplicated with stripes on the scrollbar, which allows you to locate the problem quickly.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/lines%20and%20stripes.png?raw=true" width="600">

> **Note:**
> Typos and grammatical errors are not displayed on the scrollbar.

To get information about the error, hover the mouse over the wavy line/stipe on the scrollbar. A popup with details appears, allowing you to fix the mistake.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details.png?raw=true" width="600">

### Inspecting errors in the Problems tool window

The **Problems** tool window displays a complete list of mistakes and provides a toolset for fixing errors in a more centralized way. Each listed problem has an explanation next to it and a number of the line where the error occured.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/problems%20tab.png?raw=true" width="600">

The markings in the **Problems** tool window correspond to inspection severity levels and depend on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

Additional information about inspections severity levels can be found in the [Change inspection severity](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html) section.

To locate a specific mistake in the editor, double-click the desired problem.

## Resolving errors


