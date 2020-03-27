## MYAUDIT

MYAUDIT是一个对MyBatis xml文件进行SQL提取和变量回填的自动化工具。

## 功能特点

* 与业务深度解耦，只需上传xml文件并配置开发环境的数据库信息
* 支持提取动态SQL所有组合情况下的SQL指纹
* 支持对SQL指纹按变量字段类型进行填值，以获得可执行的完整SQL，便于后续的SQL审核
* 支持 UPDATE, DELETE, SELECT等类型SQL的提取
* 目前只支持MySQL语法族的解析和变量回填
* 支持json格式的响应信息，方便外部程序的调用

## 使用场景

### 如果你是一名DBA或者运维
* 你可以将myaudit引入你们的DB运维平台，通过myaudit来全量提取xml文件中的动态SQL，在代码上线前给出优化建议，降低风险SQL的概率。
* 你可以通过myaudit来扫描代码库（包括历史代码），来提取SQL并生成代码质量报告，将未来或者历史遗留的风险SQL揪出来。

### 如果你是一名Java开发人员
* 你可以在代码开发阶段使用myaudit来全量提取xml文件中的动态SQL，并用soar等工具来生成优化报告，帮助你发现代码中的缺陷，写出更高效的SQL。

### 如果你是一名测试人员
* 你可以通过myaudit来全量提取xml文件中的动态SQL，对MyBatis xml中的SQL进行360°覆盖测试。

## 快速入门
* [安装使用](https://github.com/dbaxg/myaudit/tree/master/doc/install.md)
* [体系架构](https://github.com/dbaxg/myaudit/tree/master/doc/structure.md)
* [配置文件](https://github.com/dbaxg/myaudit/tree/master/doc/config.md)
* [操作指南](https://github.com/dbaxg/myaudit/tree/master/doc/handbook.md)

## License

[Apache License 2.0](https://github.com/dbaxg/myaudit/tree/master/LICENSE)