# 𝐂𝐍𝐍 𝐏𝐫𝐨𝐣𝐞𝐜𝐭: 𝐌𝐚𝐥𝐚𝐫𝐢𝐚 𝐂𝐞𝐥𝐥 𝐂𝐥𝐚𝐬𝐬𝐢𝐟𝐢𝐜𝐚𝐭𝐢𝐨𝐧 𝐔𝐬𝐢𝐧𝐠 𝐕𝐆𝐆19
![C ell (1)](https://github.com/Tanwar-12/Malaria-Cell-Classification-Using-VGG19/assets/110081008/55e82e50-064e-48bb-a083-21f9547c1d0c)

## 𝐈𝐧𝐭𝐫𝐨𝐝𝐮𝐜𝐭𝐢𝐨𝐧:
Malaria, a severe and widespread parasitic disease in humans, exhibits clinical symptoms as parasites infiltrate and multiply within human red cells. Transmission occurs when infected mosquitoes bite humans, releasing parasites into the bloodstream where they infect and destroy red blood cells.



### 𝐓𝐨𝐨𝐥𝐬 𝐔𝐬𝐞𝐝:
Google Colab

## 𝐃𝐚𝐭𝐚𝐬𝐞𝐭 𝐒𝐮𝐦𝐦𝐚𝐫𝐲:
This dataset comprises 27,560 PNG images of malaria-infected and uninfected cells, grouped into two classes with 13,780 images each.

#### Classes:
* Parasitized
* Uninfected
𝐓𝐚𝐬𝐤: 𝐁𝐢𝐧𝐚𝐫𝐲 𝐂𝐥𝐚𝐬𝐬𝐢𝐟𝐢𝐜𝐚𝐭𝐢𝐨𝐧
𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐏𝐡𝐚𝐬𝐞𝐬:
* Library Importation
* Data Subset Creation (Training, Testing, Validation)
* Data Processing (Prepare Training and Testing Data)
* Visualization of Training Images
* Architecture Development
* Model Compilation
* Training
* Evaluation
* Model Saving
* Prediction
* Testing
* Visualization of Test Images
## 𝐃𝐚𝐭𝐚 𝐋𝐨𝐚𝐝𝐢𝐧𝐠 / 𝐏𝐫𝐞𝐩𝐚𝐫𝐚𝐭𝐢𝐨𝐧:
Segregation into three subsets: training, testing, and validation using the split folder library.
𝐃𝐚𝐭𝐚 𝐏𝐫𝐨𝐜𝐞𝐬𝐬𝐢𝐧𝐠:
Training: 22,069 images across 2 classes.
Validation: 2,758 images across 2 classes.
Testing: 2,760 images across 2 classes.
## 𝐕𝐢𝐬𝐮𝐚𝐥𝐢𝐳𝐚𝐭𝐢𝐨𝐧 𝐨𝐟 𝐓𝐫𝐚𝐢𝐧𝐢𝐧𝐠 𝐈𝐦𝐚𝐠𝐞𝐬:
Parasitized:
Parasitized Image
![image](https://github.com/Tanwar-12/Malaria-Cell-Classification-Using-VGG19/assets/110081008/b2443cb6-af31-40d2-b472-1e215bd16fc0)

Uninfected:
Uninfected Image
![image](https://github.com/Tanwar-12/Malaria-Cell-Classification-Using-VGG19/assets/110081008/451193a0-bff2-4838-bf58-3a0323cb556c)

## 𝐀𝐫𝐜𝐡𝐢𝐭𝐞𝐜𝐭𝐮𝐫𝐞 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭:
* Utilization of VGG19 transfer learning technique to construct a malaria cell detection architecture.

* Total params: 20,074,562

* Trainable params: 50,178

* Non-trainable params: 20,024,384

**Implementation of a flatten layer to convert output into a 1D array.**

**Application of sigmoid activation function in the last FCNN layer due to the presence of only 2 classes**.

## 𝐌𝐨𝐝𝐞𝐥 𝐂𝐨𝐦𝐩𝐢𝐥𝐚𝐭𝐢𝐨𝐧, 𝐓𝐫𝐚𝐢𝐧𝐢𝐧𝐠, 𝐚𝐧𝐝 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧:
Utilization of binary cross-entropy and Adam optimizer for model compilation.
Model trained over 50 epochs with plots for training and validation accuracy, loss, and validation loss.
## 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧 𝐫𝐞𝐬𝐮𝐥𝐭𝐬:
Train Accuracy & Loss: [0.2546966075897217, 0.9057048559188843]

Testing Accuracy & Loss: [0.21056684851646423, 0.9217391014099121]
## 𝐌𝐨𝐝𝐞𝐥 𝐒𝐚𝐯𝐢𝐧𝐠:
Model saved using h5 format.
## 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧 𝐚𝐧𝐝 𝐓𝐞𝐬𝐭𝐢𝐧𝐠:
Selection of image from testing data for prediction.

Conversion of the image into an array and expansion of its dimension.

Prediction made using if-else conditions based on maximum argument.

## 𝐕𝐢𝐬𝐮𝐚𝐥𝐢𝐳𝐚𝐭𝐢𝐨𝐧 𝐨𝐟 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧𝐬:
Prediction Visualization
![image](https://github.com/Tanwar-12/Malaria-Cell-Classification-Using-VGG19/assets/110081008/0954a1aa-5c26-4826-b62d-098579252f20)








