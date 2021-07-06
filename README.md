# EquatioNet-Handwritten-equation-solver

This is a handwritten polynomial equation solver. We start off by pre-processing the input image. This involves segregation of lines(in case of multiple equations) and individual characters, 
cropping them out from the original image and resizing the new cropped image.

I've named the project EquatioNet becasue at the crux of it, lies a Convolution Neural Network trained on close to 60,000 images of digits, symbols and letters (only support x and y variables for now) which takes
as input (you guessed it!) an image and outputs the predicted letter/symbol/digit in the image!

The individual outputs are concatenated to form a string. After some careful manipulation, the string is converted to a format suitable for processing by the SymPy library. Once processesed the, 
the code outputs the answer values for the unknown variables.
