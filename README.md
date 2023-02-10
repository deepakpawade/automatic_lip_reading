# Automatic Lip Reading using deep learning techniques
## Dataset : MIRACL-VC1 https://sites.google.com/site/achrafbenhamadou/-datasets/miracl-vc1?pli=1
""Fifteen speakers (five men and ten women) positioned in the frustum of a MS Kinect sensor and utter ten times a set of ten words and ten phrases (see the table below). Each instance of the dataset consists of a synchronized sequence of color and depth images (both of 640x480 pixels).  The MIRACL-VC1 dataset contains a total number of 3000 instances.""
![image](https://user-images.githubusercontent.com/38484434/218015842-6dcec60d-2931-4633-b5fd-b25642f93c7b.png)
![image](https://user-images.githubusercontent.com/38484434/218016567-604e449d-bc12-4490-b5eb-000e1f211238.png)

We have limited the scope of the project to only predicting the words. 

## Modules
The main code cell are in the files data_genertor.ipynb and training_model.ipynb

data_generator.ipynb : Crops lips from face images and store them in the same folder structure as the original.
![image](https://user-images.githubusercontent.com/38484434/218016938-a448ca6c-390f-462c-bc57-ab79a578b1c1.png)
![image](https://user-images.githubusercontent.com/38484434/218016960-d5f2ad66-480c-4592-be29-b5a9153f8f85.png)

Extracted features:
![image](https://user-images.githubusercontent.com/38484434/218028292-d936b189-86c4-4bf3-87c0-f7b02c24ea9a.png)

training_model.ipynb : 
Model: 

![image](https://user-images.githubusercontent.com/38484434/218028768-8a767227-408c-4c34-a46f-fc42047a6eff.png)


Results:

![image](https://user-images.githubusercontent.com/38484434/218028661-6341179c-aa14-4506-95dc-64ad02a9dff2.png)


At Epoch 45, the last epoch, the Validation accuracy of the model was 0.5850 which is expected as this was a simple 3DCNN with no memory retention like RNNs. 
