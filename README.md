# FlowerClassification
a little task when learning Pytorch

the environment is very brief:

    conda create -n flowerclassification python=3.8.0
    conda activate flowerclassification
    pip install torch

    some other packages according to the "flower_division.ipynb"

this project runs on MacbookPro with M2, so I use the "mps" instead of "cuda"

## 需要注意的只有一个位置

在“10 准备训练模块”这个部分中，下面有两个cell，但是这两个cell做的是同一个事，都是实现训练函数。
第一个cell只有一个函数，就是train_model，这个是把train和test两个数据集部分通过for循环便利两次，然后在这个函数中通过if语句分开这两个部分
第二个cell有三个函数，train_epoch、test_epoch、train_model_divide，这个是分开写的写法，我觉得更清楚一点。就是把train_data和test_data要做的事分开了。
然后相应的，在“11 开始炼丹”这个部分中，就有这两个函数的分开调用，第一个注释掉的调用对应的是上面所说的第一个cell，第二个调用对应的就是第二个cell


初学Pytorch，可能还有错误的地方，继续努力...
