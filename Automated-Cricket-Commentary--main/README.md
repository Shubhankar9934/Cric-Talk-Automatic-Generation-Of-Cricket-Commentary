# Cric-Talk : Automatic Generation Of Cricket Commentary
Project Summary :
The use of artificial intelligence in sports isn’t a major surprise, given the advancement in technology. However, automated commentary is still a fantasy and the way AI and ML are developing, it could soon be a reality. The development of such a system will change the way of sports broadcasting. Hence, in this work we have tried to generate a part of automatic ball-by-ball commentary of a cricket match.\

Project Objective :
The use of artificial intelligence in sports isn’t a major surprise, given the advancement in technology. The rise in computing power, availability of massive amounts of data, and an increased willingness of stakeholders to leverage such tools are the three principal reasons why the role of artificial intelligence in sports has gained a lot more importance recently. Today every cricket lover has the freedom to analyze every ball and every shot from all possible angles, analyze how the teams fared, new milestones created, how far the ball traveled into the stands, what pace the bowlers bowled and so on – all from the comfort of their home. The impact of technology seems to have completely changed cricket’s game plan. However, the automated commentary is still a fantasy and the way AI and ML are developing, it could soon be a reality. The development of such a system will change the way of sports broadcasting. Hence, in this work, we have tried to generate a part of the automatic ball-by-ball commentary of a cricket match.\
This project contains two branches

1. Modelling
2. User-Interface

Modelling

In this folder there is Data folder and Modelling Jupyter file. In Data folder there is Images file containing link to images, Ntest.txt which is testing data, Ntrain.txt which is training data and N_token.txt which contains the image name and respective comments. For each image five different comments are written.

The model used is a basic merge model. This model uses VGG16 pre-trained model for the feature extraction from the frames and used RNN-LSTM to process the sequence of the text input. The outputs of these two models are taken as the inputs for the decoder or the merger where the inputs are merged and are processed by the dense layer for the final prediction. A few dropout layers have been implementd to reduce overfitting.




User-Interface 

Three python files namely UI_final.py, model_final.py and similarity.py We are using streamlit for creating User interface. The UI_final.py file consists of the code to create user interface. In the modelling part, we get a model for image captioning, based on this model we can predict captioning for images. While playing the video frames are considered and non similar frames are captioned. That will be the output.


