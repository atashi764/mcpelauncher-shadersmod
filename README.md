# mcpelauncher-shadersmod

This is a mod for [mcpelauncher-manifest](https://mcpelauncher.readthedocs.io/en/latest/getting_started/index.html) that allows loading RenderDragon shaders.

## Usage

‌1. Download .so file for your arch from [releases](https://github.com/GameParrot/mcpelauncher-shadersmod/releases/latest).<br><br>

![image](https://github.com/user-attachments/assets/e2cb4255-8339-48b5-9ff2-c366448a69c7)<br>
2. Open data root from here.<br><br>

![image](https://github.com/user-attachments/assets/84da268f-561a-4667-88e1-b265a7c99ce6)<br>
3. Make a folder named `mods` and place the extracted .so file there.<br><br>

![image](https://github.com/user-attachments/assets/2b378a84-a202-4d12-9b55-9f3d842de0e1)<br>
4. Put your shaders in a folder called shaders in the data root folder. RenderDragon shaders have an extension of `.material.bin`.  

<hr>

YSS shaders running with mod:  
![Shaders running](https://user-images.githubusercontent.com/85067619/233049451-6253095e-e5c9-433c-b2f3-5ccad202ecba.png)

## Building
`PATH_TO_NDK="/path/to/ndk"`
- **x86**

  ```
  cmake -DCMAKE_TOOLCHAIN_FILE=$PATH_TO_NDK/build/cmake/android.toolchain.cmake -DANDROID_ABI=x86 ..
  ```
- **x86_64**

  ```
  cmake -DCMAKE_TOOLCHAIN_FILE=$PATH_TO_NDK/build/cmake/android.toolchain.cmake -DANDROID_ABI=x86_64 ..
  ```
- **armeabi-v7a**

  ```
  cmake -DCMAKE_TOOLCHAIN_FILE=$PATH_TO_NDK/build/cmake/android.toolchain.cmake -DANDROID_ABI=armeabi-v7a ..
  ```
- **arm64-v8a**

  ```
  cmake -DCMAKE_TOOLCHAIN_FILE=$PATH_TO_NDK/build/cmake/android.toolchain.cmake -DANDROID_ABI=arm64-v8a ..
  ```
