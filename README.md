# coding2_final


# oringal movenet
https://user-images.githubusercontent.com/73170220/158729155-279b5483-04b1-4bb8-b6fc-5bd2a43527c9.mp4

For this assignment I made a movenet that monitors the movement of people in real time, but unlike a normal movenet I also added a layer of style images to render the film that it produces. The fundamental movenet uses a tensorflow model to detect and predict the movement of several key points on a person. By connecting these key points into a line, it becomes a visual and real-time Matchstick man. In the model I use it goes up to 50fps, which is very fast and easy. 
Here is the discretions of movenet model: A convolutional neural network model that runs on RGB images and predicts human joint locations of a single person. The model is designed to be run in the browser using Tensorflow.js or on devices using TF Lite in real-time, targeting movement/fitness activities. This variant: MoveNet.SinglePose.Lightning is a lower capacity model (compared to MoveNet.SinglePose.Thunder) that can run >50FPS on most modern laptops while achieving good performance. 


https://tfhub.dev/google/lite-model/movenet/singlepose/lightning/3

My original idea was to make a Matchstick man that could interact in real time and has the features of a famous painting. Wouldn't that be fun? It's like some filter, but a creepy match man. 
Next, I used one of the models from deep learning that I learned in week 8. I used it to render my live video. I thought it wouldn't be too much trouble, it didn't seem like too many steps. But I actually got stuck on the last step of rendering the live image for a long time. I using $ outputs = hub_module to force the style picture rendering the frame. And then usning $ outputs[0][0].numpy() to replace the frame that I used before. Outcome become the real-time rendering stylised video! Wa-la!



# after generation

https://user-images.githubusercontent.com/73170220/158729230-c7b00092-9168-4925-853a-f08930240d2a.mp4

However, when I change into match man only it seems much weirder. The images were difficult to render in real time and even when they finally worked it was far from what I expected. I don't know if it was a problem with the need to render frame by frame or something else, but in any case, my final product was very slow and jerky in its movement. The final matchmaker also turned out very badly, although it was amusing and funny and my friends called it the runaway hanger. But unfortunately, it didn't live up to my expectations. What's worse is that I can't find out what's wrong and I can't make any improvements for the time being. 

# only lines and keypoints been generated



https://user-images.githubusercontent.com/73170220/158729294-04568ee3-9c6f-4b1c-a03a-130d46dccae4.mp4

But I'm still glad that I made it LoL :)



