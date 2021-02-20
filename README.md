# VSCodeHelloWorld
Hello World sample for Visual Studio Code

1、工程配置文件都位于.vscode文件夹里，默认情况下，在Ubuntu的文件夹里看不到，但在VS Code里能看到，这些文件名都是不能改变的。
2、tasks.json里面用于配置构建命令，相当于Visual studio里的Build。"tasks"后面的每一个大括号里，每一个大括号里的内容就是一个Task。
3、launch.json里面用于配置启动项，相当于Visual studio里的调试运行。第一次运行找不到这个文件时会出现“Run and Debug”按钮，点击，选择
“C++(GDB/LLDB)”，自动创建launch.json。
4、打开VS Code，点击File/Open Folder，选中文件夹“VSCodeHelloWorld”
5、编译可执行程序。按“Ctrl+Shift+B”，显示“No build task to run found. Configure Build Task...”，说明还没有配置任务文件。点击刚才出现的那个
信息条，点击“Open task.json File”，出现“Select a Task Template”，选择MSBuild。因为tasks。因为tasks.json里面只有一个task，所以直接按“Ctrl+Shift+B”即可。生成的可执行文件名为“VulkanInfo.exe”。
6、运行和调试。直接按F5即可。"preLaunchTask"指定了运行前先进行的编译操作，在"label"为这个的Task。
