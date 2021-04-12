# CoNLL-Chinese
CoNLL中文数据集整理
整理CoNLL-2012中文数据集
数据来源：https://cemantix.org/conll/2012/download/
conll-2012-train.v4.tar.gz
conll-2012-development.v4.tar.gz
conll-2012-test-key.tar.gz
conll-2012-test-official.v9.tar.gz
conll-2012-scripts.v3.tar.gz
将所有数据解压在一个文档conll-2012
数据来源：https://catalog.ldc.upenn.edu/LDC2013T19
解压之后ontonotes-release-5.0

解析数据：
bash ./conll-2012/v3/scripts/skeleton2conll.sh -D ./ontonotes-release-5.0/data/files/data $./conll-2012

然后将所有数据合在一起
生成：
test.chinese.v4_gold_conll
train.chinese.v4_gold_conll
dev.chinese.v4_gold_conll
