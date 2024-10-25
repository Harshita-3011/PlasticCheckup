## Plastic Classification App

## Project Description

The Plastic Classification App is a machine learning application that uses a trained convolutional neural network (CNN) to classify different types of plastic based on images. It can help identify plastic types such as HDPE, LDPE, PET, PP, PS, PVC, and others.

So we will be collecting plastic waste from government or NGO's, segregate it and then sell it to the companies recycling plastic waste as per thier need. Like - IOC(Indian Oil Corporation) utilises PET plastic to make uniforms for its employees.

## Features

- Upload and classify plastic images.
- Real-time prediction using a trained CNN model.
- User-friendly Streamlit frontend.

## Technologies Used
- Python
- TensorFlow and Keras
- Streamlit
- PIL (Python Imaging Library)

## Pseudo Code

• Import necessary libraries: os, numpy, ImageDataGenerator, ResNet50, Dense, GlobalAveragePooling2D, Model
• Define paths to labeled image data: train_data_dir, val_data_dir
• Create data augmentation and normalization:
-train_datagen with rescaling, rotation, width shift, height shift, and horizontal flip
-val_datagen with only rescaling
• Load pre-trained ResNet50 model without the top layers
• Add custom classification head to the model:
-GlobalAveragePooling2D layer
-Dense layer with 1024 units
-Dense layer with 7 units and 'softmax' activation
• Create the final model
• Compile the model with 'categorical_crossentropy' loss and 'accuracy' as a metric
• Train the model with training data for 10 epochs and validation data
• Save the trained model to the specified path and print confirmation message

## Architecture
![377790195-1a459186-d574-410c-be80-6c359a0c7d00](https://github.com/user-attachments/assets/3f5f784c-f59f-4c75-b4d6-713ac2cf86f3)


![377790344-055823e8-1269-4c85-bf88-f338bb8452a4](https://github.com/user-attachments/assets/0c2348d3-3c50-43b0-b8f1-9ad5da555218)

## Results
 Homepage
![377788186-c5d94f1d-1191-4a2c-be3b-dcfee1de3d48](https://github.com/user-attachments/assets/be03708a-ed90-44e3-a533-298a1ed31f0f)

 Admin Dashboard
![377792461-eb135ad2-dce4-4761-ae6f-c93461e09a26](https://github.com/user-attachments/assets/dfd88cb4-ec65-47a8-8ca6-f6cb46722084)

![377792562-65c14132-0bd5-407e-8f28-52d14563cc65](https://github.com/user-attachments/assets/f8fb9437-e8c4-4788-b094-77b35bdc64c9)



