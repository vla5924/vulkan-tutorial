# Vulkan Tutorial

Vulkan SDK https://www.lunarg.com/vulkan-sdk/

Tutorial https://vulkan-tutorial.com/Drawing_a_triangle/Setup/Base_code


```bash
conan install . -s build_type=Debug --build=missing
cmake -S . -B build
cmake --build build --target triangle
```

<details>
<summary>Conan profile</summary>

```toml
[settings]
arch=x86_64
build_type=Release
compiler=clang
compiler.version=17
os=Windows

[conf]
tools.cmake.cmaketoolchain:generator=Ninja
```
</details>
