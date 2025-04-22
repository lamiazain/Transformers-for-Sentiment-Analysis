## Steps taken in this project:

### 1- Load and Explore the Dataset:
- **Load the Dataset:** I imported the IMDB dataset into my project workspace. The dataset includes labeled reviews for positive and negative sentiments, and the test subset is already provided for evaluation purposes.
- **Explore the Dataset:** I analyzed key properties, such as the distribution of sentiment labels and review lengths. Also used visualizations to better understand the dataset.
- **Split the Dataset:** I divided the "train" portion of the dataset into training and validation sets. I ensured that both subsets are representative of the overall dataset.

### 2- Implement a Data Loader:
- **Define a Custom Dataset Class:**
  - I used the PyTorch `Dataset` class to create a class that processes the IMDB data.
  - Inside the class, I tokenized the text data using the "bert-base-uncased" tokenizer. I applied padding and truncation to standardize input lengths for the model.
    
- **Build Data Loaders:**
I created `DataLoader` objects in PyTorch to handle batching and shuffling of the data for both training and validation sets.

### 3- Customize the Transformer Model:
- **Modify the Provided Model Definitions:**
  - I used the pre-written class definitions for the transformer model.
  - I filled in the missing components to adapt the model for binary classification.
  - I ensured the model outputs probabilities for positive and negative sentiments.
- **Set Hyperparameters:** I defined critical hyperparameters, including learning rate, batch size, and the number of epochs, to optimize training.

### 4- Train the Model:
- **Complete the Training Loop:**
  - I used the training dataset to iteratively update the model weights.
  - I calculated the training loss and monitored progress over epochs. 
- **Integrate Validation Steps:**
  - I evaluated the model on the validation set at the end of each epoch.
  - I tracked metrics like validation loss and accuracy to identify overfitting or underfitting. 

### 5- Test and Evaluate the Model:

- **Test on the Provided Subset:**
    - I used the pre-defined test dataset to measure the model's final performance.
    - I computed test accuracy. The test accuracy was 77%
  
By following these steps, I developed a strong understanding of transformer-based models and their application in real-world NLP tasks.

## Code Owners:
This is a guided project and part of [Udacity](https://www.udacity.com/dashboard)'s course, [Programing Transformers With Pytorch](https://learn.udacity.com/paid-courses/cd13758/lessons/f8eebe7a-536e-4e6e-887a-e178e16fc69f/concepts/6b099a04-620f-47d3-bda6-91767957be31?_gl=1*1cvwsrr*_gcl_aw*R0NMLjE3NDUxMDQ1OTYuQ2p3S0NBandrNDNBQmhCSUVpd0F2dk1FQnpZSzU0NU8wWFNDZ2JWTTIwbHdMRDNLNGR5MEpOaTNJdEZnVmkwV0NIaWJnSWZ2ZFFEWVZSb0N6XzBRQXZEX0J3RQ..*_gcl_au*MTAxMjY1ODUzOS4xNzQyNzU5NTA1*_ga*MTIzOTg3Njc0OS4xNzI3MDUzMzI1*_ga_CF22GKVCFK*MTc0NTI4NzU5My4xMTcuMS4xNzQ1Mjg3NjE4LjM1LjAuMA..&lesson_tab=lesson)

I successfully graduated and passed the course. You can review [my certificate here](www.udacity.com/certificate/e/4be8a08e-efca-11ef-a83b-a7783436f4ed)😀.
