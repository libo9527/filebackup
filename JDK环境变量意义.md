## JDK环境变量意义

JAVA_HOME

PATH

CLASS_PATH

### 环境变量

环境变量（Environment Variable）就是操作系统提供的全局变量。环境指的就是操作系统这个环境。

变量是用来被赋值/调用，环境变量也一样，不过它是整个系统环境下都可以使用，即它的作用域是整个系统！

### JAVA_HOME

指明JDK安装路径，例如：`D:\java\jdk1.8.0_08`，此路径下包括`lib`，`bin`，`jre`等文件夹（tomcat，eclipse 等都需要使用此变量）

### PATH

作用是指定 java 命令的搜索路径。我们需要把 jdk 安装目录下的 bin 目录增加到现有的 PATH 变量中，例如：`%JAVA_HOME%\bin;` bin 目录中包含经常要用到的可执行文件如 `javac`、`java`、`javaw`等，设置好 PATH 变量后，就可以在任何目录下执行这些命令了。如果不进行设置，那你就只能先进入到这个目录下，才能使用那些命令了。

### CLASSPATH

它告诉 Java 执行环境，在哪些目录下可以找到您所要执行的 Java 程序所需要的类或者包。例如：`.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar ` 通俗的说它的作用与 import、package 关键字有关，我们写的java源码中，当然会包含别人提供的工具类，比如当你写下 improt java.util.*时，编译器面对 import 关键字时，就需要知道你要引入 java.util 这个 package 中的类到底在哪里。如果不告诉，他就默认在当前目录下，而如何告诉它呢？就需要设置 CLASSPATH。只有类在 classpath 中，java 命令才能被识别。