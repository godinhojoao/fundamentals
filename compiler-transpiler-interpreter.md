## Compiler, Transpiler and Interpreter

## Compiler:

- Convert an user-friendly code into lower-level code, closer to the machine. Example: Typescript to Javascript.
- So, is Typescript considered a compiled language? Yes, and this compilation process is "static."

  ### Dynamically compiled language vs Statically compiled language

  - ### Dynamic Compiled (Java with JIT)

    - Means that the language is compiled to lower-level code (machine code) while the program is running (run-time), not before.

    ### just-in-time (JIT)

    - This allows code optimization during runtime by leveraging comprehensive information about the program's usage patterns. It identifies "hot spots" and optimizes the code based on real-time observations of the application in action.
    - This approach presents challenges for automatic benchmarking, because multiple measurements of the same program code can compare completely different machine code interpretations because the optimizer has decided to change the implementation between two runs.

  - ### Statically Compiled (Typescript)

    - Means that the language is compiled before running the program (compile time), not before.
    - When you will "build" your project using TypeScript with [tsc CLI](https://www.typescriptlang.org/docs/handbook/compiler-options.html) you are compilling your program to lower-level code, which is Javascript.

    ### Ahead-of-time (AOT)

    - Compilation occurs before running the code, generating lower-level code for execution.
    - In contrast to the Just-in-time approach, AOT typically lacks the ability to optimize based on CPU usage and real-time observations while the application is running. However, AOT achieves significant performance optimizations through inferences made during compile time.

  ### And in practice what it changes?

  - For instance, when writing or understanding a benchmark for a statically compiled language versus a dynamically compiled language, different approaches are required.
  - There are also differences related to reliability, for example, compilers can have bugs, as a developer, you may prefer encountering a bug at compile time rather than during run-time.
    - Why? If a bug is discovered during compilation, you can address it more easily without affecting your server. On the other hand, if it crashes during run-time, you might encounter more challenging issues.
  - Running a statically compiled program is generally faster than running a dynamically compiled one due to the more aggressive optimizations performed before code execution.

### Things this will help you to understand and be a better Software Developer

- When encountering terms like "run-time vs compile time," you will have a clearer understanding.
- This content that you have learned also facilitate you to understand the difference between "[Statically typed languages
  and Dynamically typed languages](https://stackoverflow.com/questions/1517582/what-is-the-difference-between-statically-typed-and-dynamically-typed-languages)".
  - Not just because of the understanding about "Dynamic vs Static", but also the knowledge about "Run time vs Compile time".
  - Even these being different contents (Typing and Compiling) they have common knowledges that are important for both.
- Now you also know that there are Compiled languages (Typescript) and Interpreted languages (Javascript).
- Frameworks such as Angular also have features related to compilation, for example, [Angular AOT compiler](https://angular.io/guide/aot-compiler), now you know the trade-offs and advantages of using it.
- Awareness of how frameworks like Angular leverage compilation, such as the use of the Angular AOT compiler. This knowledge equips you with insights into the trade-offs and advantages associated with these features.

## Interpreter

...

## Transpiler

...

> ## Thanks for reading! [Back to home](/readme.md)
