# Beautygan-pytorch
adapted from wtjiang

This is the first time I use github to upload my code. It is a bit difficult for me. Ah, what's this ? Ah, what's that?
All the code is from wtjiang. The only thing I do is putting all his files together into four .py files.

OK.Now Let us prepare the dataset.First you need to download the orignal MT-dataset.(You can find it in the paper:Beautygan).
And then establish a project below.


The project tree is like this:
1       beautygan
2      data          beautygan.py  models.py   histogram_matching.py  datasets.py

In the data:
1      data
2     makeup_dataset
3    train           val        val_MAKEMIX.txt   val_SYMIX.txt  train_MAKEMIX.txt  train_SYMIX.txt
4  images segs   images segs
5  A  B   A  B   A   B  A  B

You should put all the non-makeup images to data/makeup/dataset/train/images/A, and put all the makeup images to data/makeup/dataset/train/images/B.
You should put all the non-makeup segs to data/makeup/dataset/train/segs/A, put all the makeup segs to data/makeup/dataset/train/segs/B. 

In the train/images/A, find such files: vSYYZ450.png   vSYYZ943.png  xfsy_0068.png  xfsy_0405.png. Take them into  data/makeup/dataset/val/images/A.
In the train/segs/A, find such files: vSYYZ450.png   vSYYZ943.png  xfsy_0068.png  xfsy_0405.png. Take them into  data/makeup/dataset/val/segs/A.
In the train/images/B, find such files: 20110310_80.png   vFG112.png  vHX21.png  vRX428.png  XMY-136.png  XYUH-208.png. Take them into  data/makeup/dataset/val/images/B.
In the train/segs/B, find such files: 20110310_80.png   vFG112.png  vHX21.png  vRX428.png  XMY-136.png  XYUH-208.png. Take them into  data/makeup/dataset/val/segs/B.



