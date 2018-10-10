# Portable-camera-based-assistive-text-reader-for-blind-persons
In all, there are almost 285 million visually impaired people. About 70% among these people come from low income background. This project aims at achieving a proper portability of the entire system in a cost-effective way. A camera based text reading framework to help blind people to read texts from natural scenes from their daily lives is modelled.It deals with recognizing the surrounding objects and to interpret them accurately and giving the output in the form of speech. This paper mainly focuses on implementation of the above idea, gives approach on the challenges that we came across. It is a combination of many technologies integrated together in a marvelous way in one device to achieve the sense that was lost. Due to recent development in the image processing, speech processing, embedded system, it is possible to create an economical product to help blind people to interact efficiently with the society. As text is the important source of all information’s and decision-making skills are dependent on them, it is feasible to make it happen with this device. It is compact and small and the concept of braille notes is not that easily available and hence, it has proved very useful in real time. This device makes the senses more accurate and lead their lives easily.The whole system is made portable with Raspberry pi and output is taken from the audio jack of raspberry pi using Python and OpenCV as a platform.

Basically, the whole project is divided into three parts,
text reading only OCR
TEXT READING USING CONVOLUTIONAL RECURRENT NEURAL NETWORK
TEXT READING USING COMBINATION OF OCR + CRNN

OCR fails when,
Font is not Arial, Times new roman ,etc 
Italics
Noise in the Image
Lightning occurs                


Using CRNN TensorFlow
End to end trainable approach.
Components are separately trained and tuned.
No character segmentation or horizontal scale normalization are  involved.
Datasets involved.
Dataset used- Synth 90k [7]
Dataset is converted into TensorFlow records.


Contour sorting after extraction is the biggest problem in neural network.
Because of the variation in size of the contours of different words the extraction of text is done from any random contour and we get the speech output of random words from a single sentence.
For.eg  If the sentence is He is playing cricket it would read as  Is he cricket playing.
To overcome this disadvantage of CRNN we combine the both techniques of OCR and CRNN.

