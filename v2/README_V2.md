# Tutorial: Locate, analyze, and resolve errors

Writing code is a complex and thought-consuming process, and errors are a part of it. It is almost inevitable that at some point a mistake will be made. Lucky for us, IntelliJ IDEA analyzes our code, inspecting both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages. The system then highlights detected problems, making proofreading easier.

In this tutorial, you will learn how to locate, analyze, and resolve mistakes in your code.

## Code example

Imagine we have wrote the following code:

``` java
class Main {
    public static void main(String[] arg) {

        String[] words = { "Ruby", "C", "Python", "Java" }

        for(int i = 0; i < 3; ++i) {
            for (int j = i + 1; j < 4; ++j) {

                if (words[i].compareTo(words[j]) > 0) {

                    // swap words[i] with words[j[
                    String temp = words[i];
                    words[i] = words[j]
                    words[j] = temp;
                }
            }
        }
        // Languages appears in lexicographical order
        System.out.println("In leicographical order:");

        for(int i = 0; i < 4; i++) {
            System.out.println(words[i]);
        }
    }
}
```

The program is supposed to sort the element words in lexicographical order. However, a brief inspection of the code in the editor shows us that there are multiple errors:

<img src="https://github.com/EPprivate/private_repo/blob/main/images/errors%20in%20the%20editor.png?raw=true" width="800">

Some mistakes are not critical, but others will prevent you from running your program. We now need to 

## Locate an error

The first step to fix an error, is to locate it. You can find errors directly in the editor, since all detected problems are highlighed there. However, if you need to address multiple issues, we advise you to use the **Problems** tool window. It displays a complete list of mistakes, describes the cause behind the error, and provides a toolset to fix problems in a more centralized way.

Let's locate an error:

1. Press `Alt+6`. This key combination opens the **Problems** tool window.

2. Use the arrow keys or the mouse pointer to navigate to the desired problem.

## Examine an error

The icon near the mistake corresponds to one of the [inspection](https://www.jetbrains.com/help/idea/code-inspection.html) severity levels and depends on how serious the detected problem affects your project. The most common indicators are:

- **Error** ![error](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.balloonError.svg) - defines syntax errors.
- **Warning** ![warning](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.warning.svg) - defines code fragments that might produce bugs or require enhancement.
- **Grammar Error** ![grammar error](https://resources.jetbrains.com/help/img/idea/2022.2/grazie.icons.grammarError.svg) - defines grammar mistakes.
- **Typo** ![typo](https://resources.jetbrains.com/help/img/idea/2022.2/app.general.inspectionsTypos.svg) - defines spelling mistakes and typos.

Reviewing these markings can help you to define the cause behind the problem. It is a good practice to inspect the errors to develop a strategy for a fix before proceeding to the next step.

## Resolve an error


