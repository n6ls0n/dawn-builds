# README

A repository to host builds of the Dawn WebGPU project. See the instructions below if you want to build it from scratch.


## How to Build Dawn from Scratch on Windows

The instructions below are based on the [quick-start cmake instructions](https://github.com/google/dawn/blob/main/docs/quickstart-cmake.md) for Dawn but customized to Windows.

- Open cmd as Admin

- Clone Repo

    ```
    git clone https://dawn.googlesource.com/dawn && cd dawn
    ```

- (Optional) Checkout the commit you want to build

    ```
    git checkout <commit_hash>
    ```

- Configure w/ Cmake

    ```
    cmake -S . -B out/Release -DDAWN_FETCH_DEPENDENCIES=ON -DDAWN_ENABLE_INSTALL=ON -DCMAKE_BUILD_TYPE=Release
    ```

- Navigate to out/Release

- Double-click "Dawn.sln"

- Switch to Release in VS

- Install with VS (under CMakePredefinedTargets, right-click INSTALL project and click "Build" )

- Install with CMake

    ```
    cmake --install out/Release --prefix install/Release
    ```

## Release Info

### Release 1

- Commit hash: 474afd33
- Configuration: Default configuration for Windows
- Build Date: 9/18/24
