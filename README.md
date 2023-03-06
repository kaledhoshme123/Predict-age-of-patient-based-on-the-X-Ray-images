# Predict age of patient based on the X-Ray images
create a model capable of predicting the patient's age group through chest X-rays.
![download](https://user-images.githubusercontent.com/108609519/223055258-9b11c9cd-b3da-4373-9212-293509134bbd.png)

## Proposing a methodology of neural networks collaborating with each other:
Due to the importance of teamwork in neural networks, I suggested the following methodology, through which several neural networks can be used to predict the age of a person based on chest x-ray images for a large number of patients.
The proposed methodology is based on the existence of 4 neural networks that help each other in a specific way in order to reach the lowest value of the loss. We can summarize the proposed methodology according to the following steps:
- Model A is the model responsible for predicting the patient's age.
- Model B, another model, is also responsible for predicting the patient's age.
- Model C, another model, is also responsible for predicting the patient's age.
- Thus, we have so far 3 models out of 4, and therefore the methodology suggests that the fourth model tries to benefit from the results reached by each of the previous three models. This methodology aims to make the fourth model more capable of overcoming errors in predicting the patient’s age and making up for that difference, than By deducing the deficiency in each value that was predicted by each of the three previous models, and this is what was reached in the proposed study.
- Through which I was able to reach the lowest possible value of the loss function, the dimensions of the X-ray images included in the dataset were converted to (64, 64, 1) due to the lack of computational resources available to me.
- Thus, during the training process, Model 4 will make the three previous models output close to the correct values for the patient's age and at the same time fit with the mathematical equation that it is building, which makes it more able to reach greater accuracy in estimating the patient's age.
- In this case, we can consider model 4 as an additional control for the previous three models, and at the same time it is able to determine a more accurate value for the patient's age from the chest x-ray images.
- We can say that the fourth model is trying to identify weaknesses in each of the previous three models in order to improve the results

![download - 2023-03-06T102136 754](https://user-images.githubusercontent.com/108609519/223055485-3e04c020-291b-4118-b0f7-8b71161a80ca.png)

# Result:
![download - 2023-03-06T102643 978](https://user-images.githubusercontent.com/108609519/223056569-9d26eb1d-62ad-41f1-93fe-5c344d496ac7.png)

## Evaluate Training Data:
![image](https://user-images.githubusercontent.com/108609519/223056142-7802c83d-1bc5-493f-8def-2b8afaf6a5ee.png)
## Evaluate Testing Data:
![image](https://user-images.githubusercontent.com/108609519/223056332-20e34aee-8bd9-4370-b0c4-0694d171086e.png)

| Attempt | #1    | #2    |
| :---:   | :---: | :---: |
| Results |  ![223057118-8dccf08c-6c1f-4b2e-9852-3d38eb629cff](https://user-images.githubusercontent.com/108609519/223057463-c149c7ff-8746-4f26-bee2-50bbb7b34089.png)|              ![223057230-5f7905b8-01bc-4957-9232-00d1fd1852f3](https://user-images.githubusercontent.com/108609519/223057496-a51e0f49-7dea-418f-b48c-66621a8921bf.png)|

