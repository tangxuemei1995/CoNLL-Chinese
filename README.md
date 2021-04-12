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

'''Python
bash ./conll-2012/v3/scripts/skeleton2conll.sh -D ./ontonotes-release-5.0/data/files/data $./conll-2012
'''
然后将所有数据合在一起

生成：
test.chinese.v4_gold_conll

train.chinese.v4_gold_conll

dev.chinese.v4_gold_conll


#数据格式

#begin document (mz/sinorama/10/chtb_1041); part 000
mz/sinorama/10/chtb_1041   0   0    乐团   NN  (TOP(NP*   -   -   -   -   *   -
mz/sinorama/10/chtb_1041   0   1    讲古   NN        *))  -   -   -   -   *   -

mz/sinorama/10/chtb_1041   0    0     台湾    NR   (TOP(IP(IP(NP(DNP(NP*)  -    -   -   -    (NORP)  (ARG0*         *         *             *            *    (27|(44)
mz/sinorama/10/chtb_1041   0    1      的   DEG                       *)  -    -   -   -        *        *         *         *             *            *          -
mz/sinorama/10/chtb_1041   0    2     乐团    NN                    (NP*   -    -   -   -        *        *         *         *             *            *        (27
mz/sinorama/10/chtb_1041   0    3     传统    NN                      *))  -    -   -   -        *        *)        *         *             *            *     27)|27)
mz/sinorama/10/chtb_1041   0    4    起源于    VV                    (VP*   -   01   -   -        *      (V*)        *         *             *            *          -
mz/sinorama/10/chtb_1041   0    5     美军    NN              (NP(IP(NP*)  -    -   -   -   (DATE*   (ARG1*    (ARG0*)        *             *            *        (29
mz/sinorama/10/chtb_1041   0    6     协防    VV                   (VP*))  -   01   -   -        *        *       (V*)        *             *            *          -
mz/sinorama/10/chtb_1041   0    7     时期    NN                 (NP*))))  -    -   -   -        *)       *)        *         *             *            *    (29)|29)
mz/sinorama/10/chtb_1041   0    8      ，    PU                       *   -    -   -   -        *        *         *         *             *            *          -
mz/sinorama/10/chtb_1041   0    9      在     P                 (IP(PP*   -    -   2   -        *        *         *         *             *   (ARGM-LOC*          -
mz/sinorama/10/chtb_1041   0   10     大兵    NN        (NP(CP(CP(IP(NP*)  -    -   -   -        *        *         *    (ARG0*)            *            *        (63
mz/sinorama/10/chtb_1041   0   11     出入    VV                   (VP*))  -   01   -   -        *        *         *       (V*)            *            *          -
mz/sinorama/10/chtb_1041   0   12      的   DEC                      *))  -    -   -   -        *        *         *         *             *            *          -
mz/sinorama/10/chtb_1041   0   13     酒吧    NN                  (NP*)))  -    -   -   -        *        *         *    (ARG1*)            *            *)   (63)|63)
mz/sinorama/10/chtb_1041   0   14      ，    PU                       *   -    -   -   -        *        *         *         *             *            *          -
mz/sinorama/10/chtb_1041   0   15     现场    NN                    (NP*   -    -   -   -        *        *         *         *    (ARGM-LOC*)      (ARG0*          -
mz/sinorama/10/chtb_1041   0   16     乐团    NN                       *   -    -   -   -        *        *         *         *        (ARG0*)           *          -
mz/sinorama/10/chtb_1041   0   17     演唱    NN                       *)  -   01   -   -        *        *         *         *           (V*)           *)         -
mz/sinorama/10/chtb_1041   0   18      是    VC                    (VP*   -   01   1   -        *        *         *         *             *          (V*)         -
mz/sinorama/10/chtb_1041   0   19     必备    JJ           (NP(DNP(ADJP*)  -    -   -   -        *        *         *         *             *       (ARG1*        (53
mz/sinorama/10/chtb_1041   0   20      的   DEG                       *)  -    -   -   -        *        *         *         *             *            *          -
mz/sinorama/10/chtb_1041   0   21     背景    NN                    (NP*   -    -   -   -        *        *         *         *             *            *        (53
mz/sinorama/10/chtb_1041   0   22     音乐    NN                    *))))  -    -   -   -        *        *         *         *             *            *)    53)|53)
mz/sinorama/10/chtb_1041   0   23      。    PU                      *))  -    -   -   -        *        *         *         *             *            *          -
