# Tutorial: Locate, analyze, and resolve errors

Writing code is a complex and thought-consuming process, and errors are a part of it. It is almost inevitable that at some point a mistake will be made. Lucky for us, IntelliJ IDEA analyzes our code, inspecting both [programming](https://www.jetbrains.com/help/idea/code-inspection.html) and [natural](https://www.jetbrains.com/help/idea/proofreading.html) languages. The system highlights detected problems, making proofreading easier. This initial review can help us to eliminate the most obvious issues right away, and keep our code tidy.

In this tutorial, you will learn how to locate, analyze, and resolve mistakes in your code.

## The problem

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

Some mistakes are not critical, but others will prevent us from running the program. Our goal is to locate and resolve all detected problems. 

## Locate an error

The first step to fix an error, is to locate it. You can find errors directly in the editor, since all detected problems are highlighed there. However, if you need to address multiple issues, it is more convenient to use the **Problems** tool window. It displays a complete list of mistakes, describes the cause behind the error, and provides a toolset to fix problems in a more centralized way.

Let's open the **Problems** tool window and navigate to the first problem in the list:

1. Press `Alt+6`. This key combination opens the **Problems** tool window.
2. Use the arrow keys or the mouse pointer to navigate to the first problem in the list.

## Examine an error

After locating the problem, it is a good practice to inspect it to understand what you are dealing with. Lets take a look at the selected problem:



The description of the error tells us that the '**;**' sign is missing at the fourth line of the file. We can also gather additional information about the mistake by taking a look at the marking next to it. This icon corresponds to one of the [inspection](https://www.jetbrains.com/help/idea/code-inspection.html) severity levels and depends on how serious the detected problem affects the project. In our case, we have a syntax error.

## Resolve an error

Once we have located and reviewed the 
