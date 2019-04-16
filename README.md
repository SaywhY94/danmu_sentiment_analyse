## 利用情感词典对弹幕进行情感分析

### 使用方法：

将待处理的文件放入**raw_data**文件夹，调用脚本时输入要处理的文件名，需要处理的列，输出的文件名即可，脚本会自动在**raw_data**下生成一个**output**文件夹用于存放处理结果

```bash
python sentiment_analyse.py -i 'filename' -c 'column' -n 16
```
### 参数说明：
1. ``-i``或``--inpath``：输入excel文件的名称
2. ``-c``或``--column``：输入数据要处理的列明
3. ``-n``或``--ncores``：处理是并行的线程数
示例：python sentiment_analyse.py -i type1.xlsx -c message -n 16

如需要查看命令行参数可输入
```bash 
python sentiment_analyse.py -h
```