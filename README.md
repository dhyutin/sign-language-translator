# sign-language-translator

- Problem Description:

Over 5% of our global population, i.e, 432 million adults and 34 million children have hearing disability. One of the major difficulties faced by deaf people is their means of communication. Not everyone around the world is aware of sign-language. Although many services are deaf-people-friendly, like provision of running subtitles in cinemas, providing written instructions near shops, etc, there are not many services available that put in efforts to understand what the deaf people want to convey. 
In order to cater to the needs of deaf people and help them communicate better, there is a surging need for a mobile-sign language translation service which is handy.

- Approach:

Our main aim is to facilitate the process of sign language translation by use of various ML algorithms and models.
Our Input is an image of a hand gesture of a person communicating in sign language.
Our Output will be English Text corresponding to the translation of what the person said.

There are 4 major steps to facilitate the following:

Image Preprocessing

Identification of human hand

Train a CNN to identify hand gestures

Aim here will be to attain maximum accuracy

- Dataset:

We have chosen the Standard MINST Sign Language Dataset for testing and training purposes.
Each training and test case represents a label (0-25) as a one-to-one map for each alphabetic letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The training data (27,455 cases) and test data (7172 cases) are approximately half the size of the standard MNIST but otherwise similar with a header row of label, pixel1,pixel2….pixel784 which represent a single 28x28 pixel image with grayscale values between 0-255. The original hand gesture image data represented multiple users repeating the gesture against different backgrounds


- Model:

To train our model, we have used a Convolutional Neural Network of the following architecture:

An input layer

Convolution 

Batch Normalization

Max Pooling

Convolution 

Batch Normalization

Max Pooling

Convolution 

Batch Normalization

Max Pooling

Flatten

Hidden Layer

Output

(The model architecture is a result of trial and error based experimentation and application of basic Computer Vision backed intuition)
