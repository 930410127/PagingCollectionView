# PagingCollectionView
横向排列且横向滑动的UICollectionview  (合适点个星吧 支持一下) <br>

![](https://github.com/shengpeng3344/PagingCollectionView/blob/master/PagingCollectionView/showgif.gif)

你需要自定义layout，处理横向排列cell的逻辑，才能使collectionview按照我们的要求来排列，但并不使用系统的重排API,在自定义collectionview类中写重排逻辑 <br>
即利用collectionview的moveItemAtIndexPath:toIndexPath:接口，但前提是你要进行数据更新处理，数据源要删除，插入操作等都要先处理<br>

BUG提示:震动在切换屏时，cell重用仍会导致震动动画消失，如果不需要，可以取消震动效果

博客地址：http://blog.csdn.net/shengpeng3344/article/details/51673707
