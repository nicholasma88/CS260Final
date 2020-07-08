# Generative Adversarial Black Box
## ZOO K-lixel algorithm:
Adversarial black-box research has an important role in preventing deep neural network misclassification and recognition system obfuscation.  Several algorithms, such as Zeroth Order Optimization (ZOO) [1], One Pixel Attack [2], Adversarial Deformation [3], and Universal Perturbation [4] have been developed to create adversarial perturbations on black-box models.  In this report, we will explore the Adversarial Deformation, One Pixel Attack, and ZOO algorithms.  We then propose a black-box image classification technique that imports the combination of a One Pixel attack and k-means clustering into the ZOO algorithm.  
Our method, named ZOO K-lixel (“ZOO” + “K”-means + c“l”ustering + One P“ixel”) , reduces ZOO attack time through selectively restricting pixel locations that are subject to attack.  Our approach consists of grouping raw images by label; finding similarities between specific images through k-means clustering on each image label; running a 3 pixel attack on each image for multiple images classified to the same cluster; and identifying 40 most frequently selected pixels in each cluster.  The data set including 40 most frequently selected pixels of different clusters used to modify the original ZOO algorithm.  As compared to ZOO, our algorithm is able to achieve the same 100% attack success rate, comparable distortion (despite slightly higher), and reduced attack time. 
