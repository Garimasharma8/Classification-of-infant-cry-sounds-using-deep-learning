# Classification-of-infant-cry-sounds-using-deep-learning
Objective: We have data for infant cries for 5 different classes including tired, hungry, discomfort, burping, and belly pain. 
Challenges: The dataset is highly imbalanced, and hence applying and analyzing results would not be meaningful. 
Solution: Before designing a classifictaion model, the data from minority classes are augumented by implementing SMOTE. 

Methodology adopted: We have created spectrogram images from cry sounds and pass it to the CNN to perform classification. The CNN model proposed is: 


![image](https://user-images.githubusercontent.com/97305078/185963561-29f8e6fd-fd3b-4d15-8b98-f0673f1e528e.png)

The other parameters are: 
loss function = catergorical cross entropy, 
optimizer = adam, 
activation function = ReLu (for inner layers) and softmax (output layer), 
epochs = 100, 
batch_size = 32.

The model's accuracy and loss function's graph are:



![image](https://user-images.githubusercontent.com/97305078/185964328-544ee078-8eef-47da-8642-12798bd80a39.png)

![image](https://user-images.githubusercontent.com/97305078/185964387-a3690aa0-1acd-4f15-a14f-ce9171227579.png)

Results: 
Training acuracy = 87.77%
Validation accuracy = 82.02%
Test accuarcy = 85.39%

