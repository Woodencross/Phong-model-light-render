# 项目配置说明

由于包含了外部库，所以在此说明相关配置。

1. 项目→OpenGL_01属性→配置属性→VC++目录

   ![image-20200106120720804](D:\Files\大三\计算机图形学\Readme.assets\image-20200106120720804.png)

2. 在包含目录中添加`glm\glm`与`glfw-3.3.1\include`文件夹，若项目无法找到项目内自定义头文件，则再添加`Visual Studio 2015\Projects\OpenGL_01\OpenGL_01`文件夹

   ![image-20200106121158461](D:\Files\大三\计算机图形学\Readme.assets\image-20200106121158461.png)

3. 在库目录中添加`glfw-3.3.1\build\src\Debug`文件夹

   ![image-20200106121328198](D:\Files\大三\计算机图形学\Readme.assets\image-20200106121328198.png)

4. 选择链接器→输入，添加`opengl32.lib`与`glfw3.lib`

   ![image-20200106121535431](D:\Files\大三\计算机图形学\Readme.assets\image-20200106121535431.png)
   
5. 在项目源文件中添加现有项→`glad\src\glad.c`，此文件为在线选择OpenGL版本后自动生成。

配置完成。