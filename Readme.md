# KotlinCompileFromCmdLine

This is a repository to compile a pure kotlin project without a build system such as Gradle.

Prerequisites:
- Only use `kotlinc` compiler
- Have multiple classes under the same root package, although can have sub packages
- Be able to compile all the classes and generate an executable `jar`

## Using `kotlinc` [[Read official docs](https://kotlinlang.org/docs/tutorials/command-line.html)]

- To compile the a single kotlin file using the Kotlin compiler

```bash
$ kotlinc hello.kt -include-runtime -d project.jar
```

- To compile the a folder with multiple kotlin files under sub packages using the Kotlin compiler

```bash
$ kotlinc src -include-runtime -d project.jar
```
> where `src` has nested folders as `src/com/example/cmdline` when package is `com.example.cmdline`

## Run compiled kotlin code

```bash
$ java -jar project.jar
```

License
=======

    Copyright 2019 Nishant Srivastava

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
