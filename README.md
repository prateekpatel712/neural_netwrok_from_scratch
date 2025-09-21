#Neural Network for Recognizing A, B, and C
What This Project Is About
I built a simple neural network from scratch using only NumPy. The goal was to teach it how to recognize hand-drawn, blocky images of the letters 'A', 'B', and 'C'. This project was a great way to learn the basics of how neural networks work without using big libraries like TensorFlow or PyTorch.

How It Works
1. Creating the Letters
Instead of using a pre-existing dataset, I created the letters myself as simple black and white patterns on a 5x6 grid. Each letter is just a list of 0s and 1s, representing the 30 pixels in the image.

2. Building the Network
The network itself is pretty simple:

An input layer with 30 neurons, one for each pixel.

A hidden layer with 5 neurons to find patterns in the pixel data.

An output layer with 3 neurons, one for each letter (A, B, or C).

I used the sigmoid activation function, which helps the network make its final decision.

3. Teaching the Network
The network learns through a process called backpropagation. In simple terms:

It makes a guess about what letter it's seeing.

It checks how wrong its guess was (this is the "loss").

It goes back and adjusts its internal connections ("weights") to make a better guess next time.

This was repeated 10,000 times, which gave the network plenty of practice.

What I Found
To see how well the network was learning, I kept an eye on its loss and accuracy. The loss dropped steadily, and the accuracy climbed to 100%, which means it figured out how to tell the letters apart perfectly.

To be sure, I tested it on the letter 'B', and it got it right. The plots and the final prediction image show that the training was a success.



