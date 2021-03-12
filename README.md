# PartOfEmotect
part of Emotect (mindspore) just for debug
# part_of_Emotect
part of Emotect (mindspore) just for debug

## 环境依赖
1. Python 3 版本: 3.7.5
3. MindSpore: 1.1.1 

## 使用百度提供的一份已标注的、经过分词预处理的机器人聊天数据集，运行数据下载脚本:
```bash
sh script/download_data.sh
```
运行成功后，会生成文件夹 ```data```，其目录结构如下：

```text
.
├── train.tsv       # 训练集
├── dev.tsv         # 验证集
├── test.tsv        # 测试集
├── infer.tsv       # 待预测数据
├── vocab.txt       # 词典

```
运行数据格式转换脚本, 将数据集转为MindRecord格式:
```bash
sh scripts/convert_dataset.sh
```
