# MachineLearning

The purpose of this project was to try and create an neural network from scratch and train it to identify all letters in a picture.
For example if given a stop sign it would return STOP.

My initial idea was not to train a neural network but more of a brute force method, using the code from Lab 6 where we made a SVM classifier
I'll train it for all letters then use a sliding window on any given image, however that didn't work for multiple reasons:

1) not all letters are the same size
2) the picture can be at an angle

My next idea was to still use the SVM classifer but try to gray scale the image in question, and then split the image into smaller pieces.
Upon researching that I found: 
https://github.com/laddng/LiPlate

Where I read and tried to use that code but with little to no success

Finally with lab 8 I thought of a repsectable solution, I'll train a neural network to learn what an A looks like then given an image it should be 
able to find itself.

My research led me to this blog:
https://medium.com/@ageitgey/machine-learning-is-fun-part-3-deep-learning-and-convolutional-neural-networks-f40359318721

I wanted to put a twist on what was read their I wanted to see if given plain text of A can it detect it despite the background, I wanted 
to train the data given from Lab 6 then test it using the Flickr API images but I couldn't get my neural network to work.

I used the code from their but tried to build my own neural network to follow these layers:
1) Normalize the images
2-3) Convultize the images
4) Max pooling
5) Convultizze the image again
6) Result

However after much struggling I am unable to get the network to work, I want to train the data on the neural network on Lab 8 and see if given the 
training from that data will result in any accuracy on the Flickr API.

*I downscaled my project instead of detecting all letters I tried to only detect the letter A
