# Locating and resolving errors

While working in a file, IntelliJ IDEA analyzes your code, highlighting the sections that require a closer look. The system inspects both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages, checking syntax, spelling, and grammar. All found problems are marked in the editor and duplicated in a variety of other places, allowing you to quickly locate and resolve the issue.

## Locating errors

In IntelliJ IDEA, all error-related information is displayed:

![errors overview](https://github.com/EPprivate/private_repo/blob/main/images/errors%20overview.png?raw=true)

Markings in the editor and on the scrollbar can be used for a [brief inspection](#inspecting-errors-in-the-editor). If you want to perform a more thorough review, use the [**Problems** tool window](#inspecting-errors-in-the-problems-tool-window).

To see the statistics for detected errors, take a look at the **Inspections** widget. It displays the number of mistakes based on their <a href="#severity_levels">severity level</a>.

![inspections widget](https://github.com/EPprivate/private_repo/blob/main/images/inspections%20widget.png?raw=true)

### Inspecting errors in the editor

Inspecting errors in the editor is convenient when there are few of them. Mistakes are highlighted as red/green wavy lines and duplicated with stripes on the scrollbar, which allows you to locate the problem quickly.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/lines%20and%20stripes.png?raw=true" width="600">

> **Note:**
> Typos and grammatical errors are not displayed on the scrollbar.

To get information about the error, hover the mouse over the wavy line/stripe on the scrollbar. A popup with details appears, providing additional information about the mistake.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details.png?raw=true" width="600">

For information on how to fix mistakes, see the [Resolving errors](#resolving-errors) section.

### Inspecting errors in the Problems tool window

The **Problems** tool window displays a complete list of mistakes and provides a toolset for fixing errors in a more centralized way. Each listed problem has an explanation next to it and a number of the line where the error occurred.

To open the **Problems** window, do one of the following:

- Click the **Problems** tool below the editor.
- Click the **Inspections** widget located at the top of the scrollbar.
- Press `Alt+6`.

As a result, the **Problems** tool window opens.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/problems%20tab.png?raw=true" width="600">

<a name="severity_levels"></a>The markings in the **Problems** tool window correspond to [inspection](https://www.jetbrains.com/help/idea/code-inspection.html) severity levels and depend on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

Additional information about inspection severity levels can be found in the [Change inspection severity](https://www.jetbrains.com/help/idea/configuring-inspection-severities.html) section.

To locate a specific mistake in the editor, double-click the desired problem (or select the problem and press `F4`). Alternatively, you can open the editor preview and find the issue there. To do this, click the **Open Editor Preview** button.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/open%20editor%20preview.png?raw=true" width="600">

Once the pane is opened, select the problem that you want to inspect.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/opened%20editor%20preview.png?raw=true" width="600">
  
> **Note:**
> The opened pane acts as an normal editor, so you can modify the code or apply available fixes right there.
  
For information on how to fix mistakes, see the [Resolving errors](#resolving-errors) section.

## Resolving errors

IntelliJ IDEA analyzes all detected problems, provides a description for each error, and offers a way to fix the issue. Mistakes can be resolved either directly in the editor, or in the **Problems** tool window that allows you to process more errors at once.
  
### Fixing errors in the editor

If there are few errors in your code, you can address the problems directly in the editor. To fix a mistake, do the following:
  
1. In the editor, or on the scrollbar, [locate](#inspecting-errors-in-the-editor) the problem that you want to resolve.
2. Hover the mouse over the highlighted error or a stripe on a scrollbar. A dialog with description of the mistake opens.
	
	<img src="https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details.png?raw=true" width="600">
	
	<img src="https://github.com/EPprivate/private_repo/blob/main/images/highlighting%20details%202.png?raw=true" width="350">

3. Click the suggested fix, or press `Alt+Shift+Enter` to resolve the problem.

>Note:
>If the suggested fix is not applicable, you can see other recommendations by clicking the **More actions...** button, or pressing `Alt+Enter`.	

Alternatively, place the caret at the highlighted line, click the bulb icon ![bulb](https://resources.jetbrains.com/help/img/idea/2022.2/app.actions.intentionBulb.svg) that appears near the line counter, and select the suggested fix.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/bulb.png?raw=true" width="500">
	
### Fixing errors in the Problems tool window
	
The **Problems** tool window displays all errors that were found in the file you are currently working in, as well as on the project level. To fix the errors, do the following:

1. [Open](#inspecting-errors-in-the-problems-tool-window) the **Problems** tool window.
2. Select the mistake that you want to fix, right-click it, then choose the **Show Quick Fixes** option from the menu. Alternatively, click `Alt+Enter` once the error is selected.
	
	<img src="https://github.com/EPprivate/private_repo/blob/main/images/show%20quick%20fixes.png?raw=true" width="600">	
	
3. Select the appropriate fix from the menu.

If there are multiple similar problems, you can fix all of them at once. To do this:
	
1. Select the mistake that appears multiple times, right-click it, then choose the **Show Quick Fixes** option from the menu. Alternatively, click `Alt+Enter` once the error is selected.
2. Click the arrow button, then **Apply all '...' fixes in file**.

	<img src="https://github.com/EPprivate/private_repo/blob/main/images/fixing%20multiple%20mistakes.png?raw=true" width="600">
	
As a result, all similar problems are fixed.
	
For additional information about the actions that can be performed in the **Problems** tool window, see the [Problems tool window](https://www.jetbrains.com/help/idea/problems-tool-window.html) section.
