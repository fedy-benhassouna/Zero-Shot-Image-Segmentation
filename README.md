# Mask Generation with SAM for Protest Image

This project focuses on applying Segment Anything Model (SAM) for mask generation on an image of a protest. The goal is to identify and highlight objects in the image using advanced computer vision models.

## I. Overview

- The project leverages two models:
  1. **facebook/sam-vit-huge**: A large SAM model from Hugging Face's `transformers` library, known for high-quality segmentation results.
  2. **Zigeng/SlimSAM-uniform-77**: A slim, faster version of SAM used to improve inference speed without sacrificing too much performance.

## II. Workflow

1. **Image Loading and Preprocessing**: 
   - The protest image is loaded and resized for processing.
     ![Protest Image](https://github.com/user-attachments/assets/61d9b696-875a-466c-94aa-90ca0abf1f90)

   
2. **Mask Generation**:
   - The large SAM model is applied to generate masks for various objects in the image. The masks can be visualized for each detected object.
   ![image](https://github.com/user-attachments/assets/06fe0b4e-7e8d-444d-9393-0d4e5c021d25)

3. **Faster Inference**:
   - For quicker mask generation, the project also uses a lightweight version of SAM (`SlimSAM`), enabling faster processing with competitive results.
![image](https://github.com/user-attachments/assets/9ed0e891-ed35-4521-b8d9-e19b6e1fd25f)

## III. Tools and Libraries

- **Python**: The core programming language used for this project.
- **Transformers**: The Hugging Face library used for loading pre-trained models.
- **PyTorch**: The deep learning framework that powers model inference.
- **PIL (Python Imaging Library)**: For image handling and manipulation.
- **Matplotlib**: For visualizing results, including the generated masks.

## IV. Usage

- The project demonstrates how to generate masks on a real-world protest image, highlighting banners, people, or other relevant objects.
- It offers a comparison between a standard SAM model and a faster, slim version to optimize for either performance or speed, depending on the use case.
