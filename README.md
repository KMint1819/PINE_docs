![PINE logo](https://imgur.com/GU3kdQh.jpg)

# NOTE: Since the source code of PINE is confidential, this repository only contains the documentation and usage. 

# Pine
A web server for training machine learning models.

## Model choices
- Machine learning
    - SVM
    - KNN
    - K-means
    - Random forest
    - PCA
    - FFT

- Deep Learning
    - CNN
    - DNN
    - LSTM
    - GAN
    - AutoEncoder

## Installation
1. Clone the repository
    ```
    git clone https://github.com/KMint1819/PINE.git
    ```
2. Install dependencies
    ```
    cd PINE
    npm install
    npm rebuild
    ```
3. Configure the server
    - `$ROOT/env/development.env`
        - Adjust the `PYTHON_PATH` according to your computer.
4. Run the server
    ```
    npm start
    ```
5. Go to https://localhost:9000 from the browser
    > The port number might be different depending on the $ROOT/env/development.env file

## Training steps
This tutorial shows you how to train a iris species classifier using random forest by PINE.
1. Login to PINE or press the `create one` below to create an account.
    - ![](https://i.imgur.com/YWKKhiF.png)
2. Select the table you want to upload to.
    > You might need to request your administrator to create the table

    - ![](https://i.imgur.com/YgGKDca.png)

3. Drag your data (csv, images) to the area and wait for the progress bar to finish
    - ![](https://i.imgur.com/VKIbHk0.png)
    
    - ![](https://i.imgur.com/dxpDW7x.png)

4. Click the button at the left and choose analysis
    - ![](https://i.imgur.com/5UyYRp7.png)
    
    - ![](https://i.imgur.com/Z7FajhC.png)

5. Select your table and column attributes. 
    - This tutorial takes iris dataset for example, so we choose `petal_length`, `petal_width`, `sepal_length`, `sepal_width` for our training data.
    - ![](https://i.imgur.com/2Dyk2cd.png)
    - ![](https://i.imgur.com/ccV0YSa.png)
6. Click search and wait until the data are visualized.
    - ![](https://i.imgur.com/XydWRgd.png)
    - ![](https://i.imgur.com/WUfwyAY.png)

7. Switch to label data tab and select your table and column attributes.
    - The label data for iris is the species, so we choose `species` for our label data.
    - ![](https://i.imgur.com/nD6xWDH.png)
    - ![](https://i.imgur.com/MpneBQI.png)
8. Click search and wait until the data are visualized.
    - ![](https://i.imgur.com/QZl8EOQ.png)
9. Click the `Next` button below.
    - ![](https://i.imgur.com/FakEl94.png)
10. Choose your preprocessing method for both training data and label data.
    - For iris dataset, there is no need to preprocess the data, so we choose `None` for both data.
    - ![](https://i.imgur.com/cAgmqTJ.png)
    - ![](https://i.imgur.com/kNHH2IV.png)
    - ![](https://i.imgur.com/x0INN5B.png)
11. Click the `next` button below.
    - ![](https://i.imgur.com/tIafiD8.png)
12. Choose your model to train.
    - ![](https://i.imgur.com/L19MSZR.png)
    - ![](https://i.imgur.com/s3u6u71.png)
13. Set the hyperparameters or leave them as default value. 
    - ![](https://i.imgur.com/asEfUAn.png)
    - ![](https://i.imgur.com/cj9VtOP.png)
14. Click the `Next` button below
    - ![](https://i.imgur.com/xQf38P8.png)
15. Wait for the training result
    - ![](https://i.imgur.com/nH4TGnI.png)
    - ![](https://i.imgur.com/8fk7sT0.png)
16. Download the model by clicking the button
    - ![](https://i.imgur.com/sxxtAB2.png)
17. Extract the .zip file and you will get three files
    - ![](https://i.imgur.com/w58zo9s.png)
    - `model.pickle`: Your random forest model
    - `modelTraining.py`: Script for training the model
    - `example.py`: Example of using the model to inference data.

## Integration
- [x] RandomForest
- [x] AutoEncoder
- [x] GAN
- [x] KNN
- [x] Kmeans
- [x] PCA
- [x] LSTM
- [x] FFT
