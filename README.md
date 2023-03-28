# DrLIM
Implemention of Dimensionality reduction by learning an invariant mapping in CVPR2006
- In the abstract of MOCO, The DrLIM was introduced, which utilizes the perspective of contrastive learning.
### Loss Function.
- left expression describe "similar" and right expression describe "dissimilar" <br>
![image](https://user-images.githubusercontent.com/38518648/228127393-82d25e06-9889-4d7f-b940-38c011b5a9fe.png)

### Model Architecture

![image](https://user-images.githubusercontent.com/38518648/228127444-5cf5f356-cf05-4f28-9815-1eb4715fa9aa.png)

### Dataset

- MNIST
  - train: 3000 + a (Augmentation of -6, -3, and 3 degree rotation plus 6 pixel dropout.) of each class
  - test: 400 of each class 
- training set
  - ex) img1, img2, label. img1, img2 is random shuffle of "4" and "9". and label is write under the description.
- Using class of "4" and "9"
  - label 0: same class image
  - label 1: different class image


### Result.

![result](https://user-images.githubusercontent.com/38518648/228127577-89c8d999-9902-4ccf-a45d-531d44dbfdeb.png)
