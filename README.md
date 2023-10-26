# Windows WSL2 Kernel Build Script

## Build the latest released kernel from Microsoft's GitHub Page

###  Purpose
  - Build the latest Microsoft WSL2 kernel release to link to your current distros.

### Supported Distros:
  - Debian / Ubuntu

####  Supported architecture
  - x86_x64

###  Install info
  - Run the below command in your WSL window
  ```
  curl -Lso build-kernel https://wsl2-kernel.optimizethis.net
  sudo bash build-kernel
  ```
  
  - The new kernel will be located in the root build directory
    - The filename will be: `vmlinux`
  - Place the file `vmlinux` into a folder inside Windows `%USERPROFILE%`
    - I placed mine into the folder I created called `%USERPROFILE%\WSL2\vmlinux`

  - Create a file called `%USERPROFILE%\.wslconfig`
   
  - Visit the below website for instructions on how to link the kernel to WSL2 
    - https://learn.microsoft.com/en-us/windows/wsl/wsl-config

  - This is my personal `.wslconfig` [script](https://github.com/slyfox1186/windows-wsl2-kernel-build-script/blob/main/.wslconfig) that you can use to help understand the file formatting
