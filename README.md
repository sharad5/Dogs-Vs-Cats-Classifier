# Dogs-Vs-Cats-Classifier


[Tom&Spike]: https://i.ytimg.com/vi/Fp0aLxB4KQs/hqdefault.jpg "Tom vs Spike"

My solution to the kaggle playgorund challenge - [Dogs vs Cats Classifier](https://www.kaggle.com/c/dogs-vs-cats/)
I have used a from-scratch implementation of Resnet-50 Architecture. 
Finally, have also used the pretrained Resnet-50 architecture which gives mad accuracy.

Below is a log of the iterations for reference:
| Sno | Day      | Architecture | Layers | Batch Size | LR    | Epochs | Optimizer         | Train-Val Split | Augmentation | Regularization | Transfer Learning | Accuracy (Val) | Accuracy (Training) | GPU ? | Time Taken |
|-----|----------|--------------|--------|------------|-------|--------|-------------------|-----------------|--------------|----------------|-------------------|----------------|---------------------|-------|------------|
| 1   | 28/02/21 | Resnet       | 50     | 64         | 0.001 | 20     | Adam              | 0.25            | No           | Low            | No                | 89%            | 98%                 | Yes   | 90s/Epoch  |
| 2   | 28/02/21 | Resnet       | 50     | 32         | 0.001 | 20     | Adam              | 0.1             | No           | Low            | No                | 89.8%          | 92%                 | Yes   | 90s/Epoch  |
| 3   | 28/02/21 | Resnet       | 50     | 32         | 0.001 | 40     | Adam              | 0.1             | No           | Low            | No                | 91.34%         | 99.15%              | Yes   | 90s/Epoch  |
| 4   | 28/02/21 | Resnet       | 50     | 32         | 0.001 | 20     | Adam              | 0.1             | No           | High           | No                | 81.03%         | 94.13%              | Yes   | 90s/Epoch  |
| 5   | 28/02/21 | Resnet       | 50     | 32         | 0.001 | 40     | Adam              | 0.1             | No           | High           | No                | 90.84%         | 99.01%              | Yes   | 90s/Epoch  |
| 6   | 28/02/21 | Resnet       | 50     | 32         | 0.001 | 40     | Adam              | 0.1             | Yes          | High           | No                | 93.78%         | 94.83%              | Yes   | 5min/Epoch |
| 7   | 29/02/21 | Resnet       | 50     | 64         | 0.001 | 3      | SGD with Momentum | 0.1             | No           |                | Yes               | 98.42%         | 99.96%              | Yes   | 135s/Epoch |
