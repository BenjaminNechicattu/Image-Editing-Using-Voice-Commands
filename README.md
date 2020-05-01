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
1) Extract the files in a folder
2) Execute pyhton file _elements.py_

# About Team
- Benjamin G Nechicattu
- Done Maria James
- Albin Saji
- Akash Johny Kunnath
- Suma R
