## Npm

### --save-dev 和 --save 的区别

`--save` 会把依赖包名称添加到 `package.json`文件 `dependencies`键下，`--save-dev`则添加到`package.json` 文件`devDependencies` 键下。

`dependencies`是**运行时依赖**，`devDependencies`是**开发时的依赖**。即devDependencies 下列出的模块，是我们开发时用的。dependencies 下的模块，则是我们发布后还需要依赖的模块。

