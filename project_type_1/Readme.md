# KotlinCompileFromCmdLine

This project has a project structure as below when package is `com.example.cmdline`:


- `src`
   - `com/example/cmdline`
      - `Cake.kt`
      - `Candy.kt`
      - `Juice.kt`
      - `Sweet.kt` [has `main()`]

## Using `kotlinc` [[Read official docs](https://kotlinlang.org/docs/tutorials/command-line.html)]

```bash
kotlinc src -include-runtime -d sweet.jar 
```

## Run compiled kotlin code

```bash
$ java -jar sweet.jar

# Output
# I like the sweet stoff such as Popsicle, Blueberry Pie and Apple
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
