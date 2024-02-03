# Compiler, Transpiler and Interpreter

## Overview

- If you are here, you already know that it's extremely important to be proficient in Computer Science fundamentals.
- This article provides the essentials about compilers, transpilers, and interpreters. It will equip you with the necessary knowledge to be aware when using these approaches in development and also to know how to benchmark your systems.

> ## Compiler: (javac)

- Convert an user-friendly code into lower-level code, closer to the machine. Example: Java to bytecode.
- So, is Java considered a compiled language? Yes, it is. There are various types of compilation processes, as illustrated above.

### Dynamically compiled language vs Statically compiled language

  - ### Dynamic Compiled (Java with JIT)

    - Means that the language is compiled to lower-level code (machine code) while the program is running (run-time), not before.

    ### just-in-time (JIT)

    - This allows code optimization during runtime by leveraging comprehensive information about the program's usage patterns. It identifies "hot spots" and optimizes the code based on real-time observations of the application in action.
    - This approach presents challenges for automatic benchmarking because multiple measurements of the same program code can compare completely different machine code interpretations because the optimizer has decided to change the implementation between two runs.

  - ### Statically Compiled

    - Means that the language is compiled before running the program (compile time) that is before run-time.

    ### Ahead-of-time (AOT)

    - Compilation occurs before running the code, generating lower-level code for execution.
    - In contrast to the Just-in-time approach, AOT cannot typically optimize based on CPU usage and real-time observations while the application is running. However, AOT achieves significant performance optimizations through inferences made during compile time.

### And in practice what did it change?

- For instance, when writing or understanding a benchmark for a statically compiled language versus a dynamically compiled language, different approaches are required.
- There are also differences related to reliability, for example, compilers can have bugs. As a developer, you may prefer encountering a bug at compile time rather than during run-time.
  - Why? If a bug is discovered during compilation, you can address it more easily without affecting your server. On the other hand, if it crashes during run-time, you might encounter more challenging issues.
- Running a statically compiled program is generally faster than running a dynamically compiled one. Due to the more aggressive optimizations performed before code execution.

> ## Transpiler

- Compiles code to a similar level of abstraction, because of that the Transpilers are also called "Source-to-Source Compilers".
- It takes source code written in one language and translates it into equivalent code in another language at a similar level of abstraction.
- So is a Transpiler a type of Compiler? Yes. Examples of transpiled languages:

  - Babel (ES6+ to ES5) - enables writing ES6 code while supporting older browsers like IE 11 and below.
  - Typescript to javascript.
  - Flutter to javascript.

### And in practice what did it change?

  - We require a transpiler because the process of converting a substantial program into a different language is a time-consuming task.
    - Economically, it's not a good idea to spend all the time of a developer team recoding an entire software into another language.
  - This is also important for web browser compatibility.
  - We can develop cross-platform software using Flutter by converting it to JavaScript.
    - If to read every foreign research paper, we had to understand the foreign language, then it would take a lot of effort. Life without a translator is hard, and so is without a transpiler.

> ## Interpreter

- Interprets the source code without converting it to a lower-level code.
  - Example of interpreter: Ruby MRI.
- It is more convenient for the user to execute the source code with a single command. But you need the interpreter installed in your environment.

> ## Things this will help you to understand and be a better Software Developer

- When encountering terms like "run-time vs compile time," you will have a clearer understanding.
- This content that you have learned also facilitates you to understand the difference between "[Statically typed languages
  and Dynamically typed languages](https://stackoverflow.com/questions/1517582/what-is-the-difference-between-statically-typed-and-dynamically-typed-languages)".
  - Not just because of the understanding about "Dynamic vs Static", but also the knowledge about "Run time vs Compile time".
  - Even though these are different contents (Typing and Compiling) they have common knowledge that is important for both.
- Now you also know that there are Compiled languages (Typescript) and Interpreted languages (Javascript in the browser).
- Frameworks such as Angular also have features related to compilation, for example, [Angular AOT compiler](https://angular.io/guide/aot-compiler), now you know the trade-offs and advantages of using it.
- Awareness of how frameworks like Angular leverage compilation, such as the use of the Angular AOT compiler. This knowledge equips you with insights into the trade-offs and advantages associated with these features.
- You will also understand some of the usages/advantages of each approach, for example:
  - Compilers: Code optimization, Platform-specific Optimization, and more.
  - Transpiler: Cross-platform applications, Browser compatibility, code migration, and more.
  - Interpreters: Convenience in Development, Dynamic Typing, faster to debug, and more.

## Thanks for Reading!

- Feel free to reach out if you have any questions, feedback, or suggestions. Your engagement is appreciated!

## Contacts

- You can find this and more content on:
  - [My website](https://godinhojoao.com/)
  - [GitHub](https://github.com/godinhojoao)
  - [LinkedIn](https://www.linkedin.com/in/joaogodinhoo/)
  - [Dev Community](https://dev.to/godinhojoao)

[Back to home](/readme.md)
