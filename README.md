# Lilium Toolchain
Lilium Toolchain is an LLVM and Clang compiler toolchain tailored for Android kernel development, integrating LTO (Link Time Optimization), PGO (Profile Guided Optimization), and BOLT. It leverages the latest updates from LLVM's main branch to ensure optimal performance and compatibility.

## Features
- **LLVM and Clang**
Utilizes the latest LLVM compiler infrastructure and Clang front-end for robustness and modern language support.

- **LTO (Link Time Optimization)**
Enhances performance by optimizing across object files during linking.

- **PGO (Profile Guided Optimization)**
Improves performance based on profiling data, optimizing hot code paths.

- **BOLT**
Utilizes Binary Optimization and Layout Tool for further performance enhancements.

- **Integrated Binutils**
Includes binutils directly, eliminating the need for a separate GCC Toolchain. The binutils are built from the latest stable source code for reliability and efficiency.

## Getting Started

### Installation
1. **Download the Toolchain**
    - Navigate to the [Releases](https://github.com/liliumproject/clang/releases) page.
    - Download the latest .tar.gz archive.

2. **Extracting the Toolchain**
    - Use your preferred method to extract the downloaded .tar.gz archive.
        ```
        tar -xf lilium-toolchain-vX.X.X-linux-x86_64.tar.gz
        ```

3. **Setting Up Environment Variables**
    - Add the extracted directory to your PATH environment variable to make the tools accessible from anywhere in your terminal.
        ```
        export PATH=/path/to/extracted/lilium-toolchain/bin:$PATH
        ```

    - **Optionally**, you can add this line to your shell's configuration file (e.g., .bashrc, .zshrc) to make the change permanent.

4. **Verify Installation**
    - Open a new terminal window or run source on your configuration file to apply changes.
    - Check if the toolchain is correctly installed by running:
        ```
        clang --version
        ```
    
    This should display the version of Clang included in Lilium Toolchain.
