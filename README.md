# Greek_language_handwritten_recognition
This project aimed to create a neural network identifying handwritten text with the Greek alphabet.
### Project Motivation 
Handwriting recognition is proving to be a very popular neural network-related topic. However, nearly all handwriting recognition networks are limited to recognizing the Latin alphabet. My research found that there aren't many handwriting recognition networks that can recognize the Greek alphabet. Therefore, I propose creating a neural network identifying handwritten text with the Greek alphabet.
The Greek language is the official language of Greece, where it is spoken by 99% of the population, and one of the official languages of Cyprus where Greek Cypriots mostly use it. Only 0.18% of the world’s population speaks Greek. The map below shows countries with significant Greek populations and descendants (+1,000,000; +100,000; +10,000: +1,000).  
- ![#142B5F](https://via.placeholder.com/15/142B5F/142B5F.png) `+1,000,000`
- ![#2B5A9A](https://via.placeholder.com/15/2B5A9A/2B5A9A.png) `+100,000`
- ![#3875D1](https://via.placeholder.com/15/3875D1/3875D1.png) `+10,000`
- ![#9CC5EE](https://via.placeholder.com/15/9CC5EE/9CC5EE.png) `+1,000`

<img width="603" alt="Screenshot 2022-09-02 at 16 19 18" src="https://user-images.githubusercontent.com/46090129/188096491-33aed6e6-94fb-487e-ab81-9640db9dcee7.png">

There are very few handwriting recognition networks that work with Greek because the Greek language is not as popular as other languages (English, French, German).  Despite this, Greek handwriting is essential because Greek letters are commonly used in mathematics, science, and engineering. So handwriting recognition networks of Greek handwriting will help understand math/science/engineering papers.

### Data collection
It has been found out that there are not a lot of handwritten examples on the internet. Have been found papyrus data, but it cannot be used because it’s not modern Greek. To solve the problem with the lack of data most of the data have been made manually. At the end have been made dataset with different types of handwritten from different people (native, non greek speakers), that providing big variety of the examples. 

### Pre-processing 

#### data cleansing 
The process of data cleansing was done manually instead of automating it using Python code  to ensure that all data was thoroughly checked by eye to ensure it is suitable for use in  neural networks and because the automated cleansing process might throw up false positives and negatives regarding what is important data and must be kept, and what is noise and thus can be removed.
Steps in data cleansing included: 
- removing excess symbols and noise
- Thresholding
- Addressing incomplete data segments

#### Data preparation
Data preparation have been done using PyTorch. Data preparation including:
- Cropping
- Labelling
- Reshaping

### Implementation 
This task have been implemented with different neural networks to compare further which one showing better results. 
Have been used MLP, ANN, CNN, RNN. ANN showed the best results on the test set. 
