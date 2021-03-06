# Lab 5 myshell2

## Team

 - [Danylo Sluzhynskyi](https://github.com/sluzhynskyi)
 - [Marian Dubei](https://github.com/MarianDubei)
 - [Taras Rumezhak](https://github.com/tarasrumezhak)
## Prerequisites

 - **C++ compiler** - needs to support **C++17** standard
 - **CMake** 3.15+
Dependencies (such as development libraries) can be found in the [dependencies folder](./dependencies) in the form of the text files with package names for different package managers.

## Installing

1. Clone the project.
    ```bash
    git clone https://github.com/sluzhynskyi/myshell2.git
    ```
2. Install required packages.

   On Ubuntu:
   ```bash
   [[ -r dependencies/apt.txt ]] && sed 's/#.*//' dependencies/apt.txt | xargs sudo apt-get install -y
   ```
   On MacOS:
   ```bash
   [[ -r dependencies/homebrew.txt ]] && sed 's/#.*//' dependencies/homebrew.txt | xargs brew install
   ```
   Use Conan on Windows.
3. Build.
    ```bash
    cmake -Bbuild
    cmake --build build
    ```
3. Build.
    ```bash
    cmake -G"Unix Makefiles" -Bbuild
    cmake --build build
    ```

