# Searching for errors

While developing an application, IntelliJ IDEA analyzes your code, highlighting the sections that require closer look. The system inspects both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages, checking syntax, spelling, and grammar. All found problems are marked in the editor and duplicated in a variety of other places, allowing you to quickly locate and resolve the issue.

## Locating errors

In IntelliJ IDEA, mistakes are highlighted in the editor, as well as on specific widgets/windows that provide additional control options. All error-related information is displayed:

// IntelliJ IDEA highlights errors directly in the editor and duplicates all related information in a variety of places, making it easier to find and correct the mistakes. All relevant information is displayed:

![errors overview](https://github.com/EPprivate/private_repo/blob/main/images/errors%20overview.png?raw=true)

The **Inspections** widget, located at the top of the scrollbar, displays the overall amount of errors in the file.

![inspections widget](https://github.com/EPprivate/private_repo/blob/main/images/inspections%20widget.png?raw=true)

Clicking the widget opens the **Problems** tool window.

### Inspecting errors in the editor

Errors in the editor are highlighted:

- As red/green wavy lines

  ![errors as wavy lines](https://github.com/EPprivate/private_repo/blob/main/images/errors%20as%20wavy%20lines.png?raw=true)
  
- As stripes on the scrollbar

  ![stripes on a scroll bar](https://github.com/EPprivate/private_repo/blob/main/images/stripes%20on%20a%20scroll%20bar.png?raw=true)
  
   > **Note:**
   > Typos are not shown on the scrollbar.

To get information about the error, hover the mouse over the wavy line/stipe on the scrollbar. A popup with details appears, allowing you to fix the mistake, or perform other actions.

![highlighting details](https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details.png?raw=true)

![highlighting details 2](https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details%202.png?raw=true)

### Inspecting errors in the Problems tool window

The **Problems** tool window displays a complete list of mistakes and provides a toolset for fixing errors in a more centralized way. Each listed problem has an explanation next to it and a number of the line where the error occured.

![problems tab](https://github.com/EPprivate/private_repo/blob/main/images/problems%20tab.png?raw=true)

The markings in the editor correspond to inspection severity levels and depend on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

Additional information about inspections severity levels can be found in the [Change inspection severity](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html) section.

To locate a specific mistake in the editor, double-click the desired problem.

## Resolving errors


