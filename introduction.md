# 论文的冷启动消歧（Name Disambiguation from Scratch - sna）
## 数据集：训练集  验证集
### 训练集（train）
train_author.json   train_pub.json
- train_author.json:此文件中的数据组织成一个字典（dictionary，记为dic1），存储为JSON对象。 dic1的键（key）是作者姓名。 dic1的值（value）是表示同名作者集合的字典（记为dic2）。 dic2的键（key）是作者ID， dic2的值（value）是该作者的论文ID列表。
- train_pub.json:包含train_author.json所有论文的元数据,数据表示为一个字典（dictionary），其键（key）是论文ID，其值是相应的论文信息
### 验证集（sna_data）
- sna_valid_author_raw:二级字典，key值为作者姓名，value为一个论文的list，代表该作者姓名下所有同名作者的论文
- sna_valid_pub:代表验证集所有论文的元信息
- sna_valid_example_evaluation_scratch:示例提交文件，组织成二级字典格式，key值为作者姓名， value值是一个二维列表，第一维的长度代表类簇的数目，第二维代表各个类簇的论文ids
