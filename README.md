# Tutorial: Locate, analyze, and resolve errors

Writing code is a complex and thought-consuming process, and errors are a part of it. It is almost inevitable that at some point a mistake will be made. Lucky for us, IntelliJ IDEA analyzes our code, inspecting both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages. The system highlights detected problems, making proofreading easier. This initial review can help us eliminate the most obvious issues right away, and keep our code tidy.

In this tutorial, you will learn how to locate, analyze, and resolve mistakes in your code.

## The problem

Imagine we have the following application:

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

Some mistakes are not critical, but others will prevent us from running the program. Our goal is to locate and resolve all detected problems. 

## Locate an error

The first step to fix an error, is to locate it. You can find errors directly in the editor, since all detected problems are highlighted there. However, if you need to address multiple issues, it is more convenient to use the **Problems** tool window. It displays a complete list of mistakes, describes the cause behind the error, and provides a toolset to fix problems in a more centralized way.

Let's open the **Problems** tool window and navigate to the first problem in the list:

1. Press `Alt+6`. This key combination opens the **Problems** tool window.

    <img src="https://github.com/EPprivate/private_repo/blob/main/images/problems%20tool%20window.png?raw=true" width="800">

2. Use the arrow keys or the mouse pointer to navigate to the first problem in the list.

## Examine an error

After locating the problem, it is a good practice to inspect it to understand what you are dealing with. Let's take a look at the selected problem:

<img src="https://github.com/EPprivate/private_repo/blob/main/images/inspecting%20errors.png?raw=true" width="850">

We can gather information about the mistake by reviewing the description provided by the system, and the marking next to it. The icon corresponds to one of the [inspection severity levels](https://www.jetbrains.com/help/idea/code-inspection.html) and depends on how serious the detected problem affects the project. In our case, we have a syntax error: the '**;**' sign is missing at the fourth line of the file.

Also, you might have noticed that we have an identical syntax error on the thirteenth line. Since IntelliJ IDEA supports processing similar mistakes at once, we will deal with both errors during the next step.

## Resolve an error

Once we have located and reviewed the mistake, it is time to fix it. IntelliJ IDEA not only analyzes your code for errors, it also suggests how to fix them. Let's resolve our problem using the suggested fix:

1. While in the **Problems** tool window, press `Alt+Enter`. A menu with quick fix options opens.

    <img src="https://github.com/EPprivate/private_repo/blob/main/images/suggested%20fix.png?raw=true" width="850">

    We can apply the suggested fix right away, but let's also address a similar syntax error located at the thirteenth line.
    
2. Press the right arrow key.

    <img src="https://github.com/EPprivate/private_repo/blob/main/images/fix%20all.png?raw=true" width="350">

3. Press `Enter` to apply the suggested fix to both problems.

As a result, we have just resolved two similar errors at once. However, we still have two more problems. Now, that you are familiar with the general flow, let's fix the rest of the errors. To recap, you need to:

1. [Locate and navigate](#locate-an-error) to the mistake that you want to resolve.
    
    <img src="https://github.com/EPprivate/private_repo/blob/main/images/fixing%20other%20errors.png?raw=true" width="850">
    
2. [Examine](#examine-an-error) the error to gather information about it.

3. [Resolve](#resolve-an-error) the problem ussing the suggested quick fix.

    <img src="https://github.com/EPprivate/private_repo/blob/main/images/quick%20fix%20options.png?raw=true" width="850">

Once you fix the rest of the issues, the green checkmark will be displayed in the top-right corner of the editor, meaning that there are no more problems in your code.

<img src="https://github.com/EPprivate/private_repo/blob/main/images/no%20problems%20found.png?raw=true" width="350">

## Things to consider

Even if the system tells you that there are no more problems in your code, this does not guarantee that your program will provide the expected result once executed. There might be no syntax errors, however, there may be problems with logic which will affect the end result. To see what can be done in such situation, take a look at the [Debugging](https://www.jetbrains.com/help/idea/debugging-your-first-java-application.html) section.
