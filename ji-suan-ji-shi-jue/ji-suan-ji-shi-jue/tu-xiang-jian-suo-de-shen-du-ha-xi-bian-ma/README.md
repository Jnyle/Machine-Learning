# 图像检索的深度哈希编码

图像检索，就是指给定一张待搜索图片，从数据库里面检索出相似图片的过程，如[Google Images](https://images.google.com/)。为了满足实时性的搜索要求，一般会提取出图片特征并以0、1的哈希编码来压缩代替，这样就可以进行高效的检索了。随着互联网相关技术的发展，数据库的容量也越来越大，这在检索时就要求对哈希编码的位数加以控制。常用的位数选择为24位、48位和64位。因此，如何得到有效的哈希编码，就成了图像检索中的关键点。

首先，我们简单看一下传统的哈希编码方法，然后介绍如何应用深度学习来进行哈希编码，以及它所带来的优势。

