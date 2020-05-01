# Image-Manipulation-over-Voice-Commands
voice commands are used for basic image editing. We call it Elements. Elements is capable of Edit images all over voice commands.

# Welcome to Image Editing Using Voice Command.

## Abstract
Image editing encompasses the processes of altering images, whether they are digital photographs, traditional photo-chemical photographs, or illustrations. Traditional analog image editing is known as photo retouching, using tools such as an airbrush to modify photographs or editing illustrations with any traditional art medium. Graphic software programs can be broadly categorized into vector graphics editors, raster graphics editors, and 3D modelers. _This software is a primary tool with which a user may manipulate, enhance, and transform images_. Many image editing programs are used to render or create computer art from scratch via direct interaction. **We use voice commands and direct interaction to edit Images.**

## Introduction 
Image editing from scratch has become a timeconsuming process for non-professionals as well as for upgrading professionals. _Learning chunks of shortcuts and completely accessing editing tools via mouse and keyboard has become difficult, timeconsuming, and particularly overhead for at least a few_. Here, **we introduce an image editing interface that comprises of vocal command recognizer**, however, image editing is difficult to perform with voice alone.  For flexible and easy editing-control _we use both voice and manual editing interaction_, using mouse and keyboard. Selecting an object or a layer within the workspace has become easier. The editing panel is a grid fashion workspace and x-y axes (rulers) are scaled for selection of points at the workspace where an image is to be edited. This application contains an image storage directory linked to the desktop so that importing images becomes easy which is already in the application storage. There are combinations of filters that provide a professional touch to the images. Elements like adding texts and formatting, color-comb are add-on features. The functions with varying values can be adjusted in percentage/values by saying it while specifying the arguments. **Voice interface makes complex tasks easier and accessible as they allow users to simply state goals without learning an interface.**

# Image Manipulation Operations 

The usage of **pillow **library brings up a large space for image editing. Among them, few are loaded into the application. 

### Rotation. 
Rotation operation rotates the image in the workspace window. The user can specify the angle to which the image has to be rotated.  

### Brightness. 
Users can now change the brightness by saying change brightness. Brightness too needs a parameter. A floating point number is passed as the argument for brightness which in turn increase the brightness by that much. 

### Contrast.
Contrast increases the contrast of the image by a floating point value. 

### Saturation.
This operation Increase the saturation of the image or reduces the saturation. 

### Flip.  
Flips the image left to right or up to down. This makes the image looks like mirrored or tilted upside down. 

### Warmth.
Increases the red in every pixel and makes the image warmer. 

### Text. 
Now we can add text in to an image. When the text function is called, it asks for the sentence to be added in the image. Varity of fonts are also incorporated along. Font type has to be specified by specifying the font name. Position of the text in the image has to be specified by passing the x, y coordinates or by saying how much to right or down. 

### Black and white filter. 
Now a days black and white images brings nostalgic feel to the image. This can be brought to the image by a call and specify the strength of the filter.  

### Sharpness. 
Increases the sharpness of the image and makes the image crispier and less blurred. 

### Detail.
Increases the details and the structure of the objects in the image. 

### Crop. 
Crop the image by passing four arguments corresponding to left, upper, right and lower of the image.  

### Blur.
Blurs the image or reduces the sharpness of the image which gives a spread appearance to the image. 

### Contour.
This can select the pixels with same intensity and find out the edges in an image. 

### Edge Enhance.
Edge enhance enhances the edges of objects in an image. For more edge enhance use more edge enhance 
  
### Smooth.
Just like blurring, this function smoothens the objects in the image. For more smooth use more Smooth. 

### Resize. 
This function reduce the image size, resolution thus reducing the memory space occupied by the image while saving. 

### Save.
Save function saves the image in a specific name and extension format as the user specify in a user space.

# Program Execution Flow 

The Program begins when the application is open. The application welcomes the user with a splash screen. Soon after the application files and libraries are loaded it checks for internet access. If internet access is available the mic gets activated and listens for a ‘do’ command. After a ‘do’ audio fingerprint is detected you can say any command to be performed in the image. 
Selecting the image is much easier with an in-app file browser which shows the images within the PC. All you have to do is to say the name of the image or select the image manually.  The selected image is brought to the workspace window. Where you can perform image editing. Now we need to say what operation had to be performed on the image. It is a command. The command is then converted to its corresponding text via Google's Speech Recogniser API. API returns the corresponding text.

![Sequence Diagram](https://drive.google.com/file/d/1rhAq5zh8NeryhqP5XXnPoUd9YpHIp5se/view?usp=sharing)
  
The command is now tokenized to tokens. For every token, compares to a keyword in the keyword file. If the token found, calls the corresponding function and perform the action. Else if no token is found in the keyword file, the token is compared with a similar file, to avoid miss predictions. If a similar keyword is found. Then the corresponding function to the ‘similar keyword’ is called and then performs the action on to the image. For some functions, arguments are needed to be passed. For instance, say angle for rotation. When a rotation function is called, an argument has to be passed, angle. Now it’s turn for the argument to be listened and is passed to the function. We can perform enough actions on the image until a save or 
quit command appears. Save command confirms the edited image and saves the image in new name and a new extension as the user prefer. Quit command quits the image editing window without saving the changes. 

# Technologies Used 
## Python 
Core Programming is based on Python Programing language which is more convenient flexible and fast. Python is more understandable as well as readable. Execution and complexity of the program are comparatively easier and less respectively. Python is an interpreter language which helps in sequential execution if the program. 

## Tkinter Python GUI 
Python has Tkinter GUI which makes combining the scripts together. This makes it executable on any machines that have python within thus making the program cross-platform. 

## Pillow Library 
The Python Imaging Library adds image processing capabilities to the Python interpreter. Basically every operation on the image can be done using this pillow library. This gives wide file format support, an efficient internal representation, and fairly powerful image processing capabilities. PhotoImage and BitmapImage interfaces help to show the image. The library also supports image resizing, rotation, and arbitrary affine transform. 

## Natural Language toolkit 
Natural Language toolkit is used in order to get the speech and convert it to a machine-understandable form so that the machine can make meaning from it. Every command that is given to the system is tokenized by the NLTK and this enables the system to find out what operation is to be done on the image taken.
 
## Google Speech Recognition Engine 
Google speech recognition engine coverts the speech that is captured to the corresponding text. This text is then used by the Natural Language Toolkit (NLTK). The Speech is recorded by the system and acquires Google API for speech recognition and uploads the speech to generate the corresponding text. 

# Installing Packages
-  # Tkinter
-       pip install tkinter
- # Pillow
-       pip install pillow
- # Pygame
-       pip install pygame
- # NLTK
-       pip install nltk
- # IPython
-       pip install ipython
- # Speech Recognition
-       pip install speechrecognition
- # Pyaudio
-       pip install pyaudio
- # Keyboard
-       pip install keyboard

# Running the Program
-1) Extract the files in a folder
-2) Execute pyhton file _elements.py_

# Conclusion
We introduced **ELEMENTS**, A multimodal interface system to support image editing tasks through voice and direct manipulation. Other than editing functionalities "Elements" is enabled with a browsing of an image as well as saving an image after editing. We can browse our file manager or even the internet by using appropriate voice commands. After editing the procedure is the complete user can save the image using the "save" command and we can specify the appropriate location as well as the name in which image is to be saved. Thereby implementing each functionality with voice. Coming to the editing functionalities we have implemented all the features that are essential for an editing tool. Features include brightness, Contrast, crop, rotate, a total of 9 filters etc., and all these using voice commands. "Elements" have an add on functionality of image compression. Image that we select for editing maybe of larger size and we can compress them after according to our requirement, compression ratio is on a scale of 0-100. The key feature that makes "Elements" unique from other editing tools is that it is voice enabled, as it is voice controlled it can be used by the "differently abled people". Voice commands are less complex than shortcuts and is has a user-friendly UI which all makes it easy to use. So now editing is no more a complex task just tell what to do and it’s done. 
References 

# About Team
- Benjamin G Nechicattu
- Done Maria James
- Albin Saji
- Akash Johny Kunnath
- Suma R
