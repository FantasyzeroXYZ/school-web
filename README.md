# 学校课程练习
* asp.net配置
  * vscode
    * 插件
      * C# Dev Kit
      * vscode-solution-explorer
    * 安装.NET
      * 官网 https://dotnet.microsoft.com/zh-cn/
      * SDK安装
      * 重新启动vscode
    * 创建.NET项目
      * 图形化操作方式
        * `ctrl+shift+P`呼出vscode命令栏
        * 输入`.NET: Project`
        * 选择要创建项目的类型
        * 为项目命名
      * [ ] 命令行操作方式
        * `dotnet new list`
        * `dotnet new 名称 -o 指定文件路径`
        * 创建项目`dotnet new`
    * [ ] .NET其他操作
      * 查看.NET版本`dotnet --version`
      * 生成项目及其所有依赖项
        * `dotnet build`
      * 运行项目
        * 在项目路径下输入`dotnet run`
        * `Ctrl+C`退出项目运行
      * 部署项目到本地文件
        * `dotnet publish -o 文件路径`
  * visual studio
    * 官网 https://visualstudio.microsoft.com/zh-hans/
    * [ ] 安装
    * 创建新项目
      * 选择`ASP.NET Web应用程序(.NET Framework)`
      * 设置项目路径以及选择框架
      * 选择模板
        * 学校课程用`Web Forms`
    * win10开启IIS管理器
      * 参考解决方案 https://blog.csdn.net/yuanxiang01/article/details/104490141
      * `win+Q`搜索`控制面板`
      * 点击`程序`
      * `启用或关闭Windows功能`
      * 找到并勾选`Internet Information Services`
    * 发布项目
      * 在`解决方案资源管理器`里右键点击项目，选择`发布`
      * 课程要求:选择`文件夹`
      * 设置发布文件存储的路径
      * 点击`发布`
      * `win+Q`搜索`IIS`启动IIS管理器
      * 在`连接`栏里右键点击，选择`添加网站`
      * 设置`网站名称`，`物理路径`和`IP地址`
        * `物理路径`一般设置在发布的文件夹里
        * `IP地址`选择`全部未分配`
      * 在浏览器访问项目网页
        * 遇到的问题
          * 由于权限不足而无法读取配置文件
            * 参考 https://blog.csdn.net/qubernet/article/details/88943288
            * 右键点击发布部署所在的文件夹，选择`属性`
            * 切换到`安全`栏，点击`添加`
            * 在`输入对象名称来选择`里输入`Everyone`
            * 在`Everyone的权限`里的允许列上都打勾
            * 点击`应用`，然后点击`确定`
        * 设置默认文档
          * 使用此功能指定当客户瑞未请求特定文件名时返回的默认文件。按优先级顺序设置默认文档。
          * 设置自定义文件为默认需要用此设置
          * 参考 https://blog.csdn.net/Helloxiaovv/article/details/104322377
* ASP.NET官方文档 https://learn.microsoft.com/zh-cn/aspnet
* dotnet命令参考 https://learn.microsoft.com/zh-cn/dotnet/core/tools/dotnet
* ASP.NET Core应用发布
  * 参考
    * https://learn.microsoft.com/zh-cn/visualstudio/deployment/quickstart-deploy-aspnet-web-app?view=vs-2022&tabs=azure
    * https://learn.microsoft.com/zh-cn/aspnet/core/tutorials/publish-to-azure-webapp-using-vscode?view=aspnetcore-8.0
