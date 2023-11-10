# PNG_Finding_and_Concatentation
A directory encompassing both PNG and non-PNG files is provided, including nested sub-directories. Valid PNG images within this directory are horizontal strips of a larger composite image, sharing a common width but varying heights. The PNG images adhere to the naming convention *_N.png, where N represents the sequence number (N=0, 1, 2, ...). However, files with .png or .PNG extensions may not necessarily be genuine PNG image files. The task involves identifying and extracting all authentic PNG image files within the given directory. Subsequently, these images are concatenated in sequential order based on the sequence number in the file name, reconstructing the original complete image. The sequence number dictates the vertical concatenation order, with lower numbers corresponding to the upper position. For instance, img_1.png is the initial horizontal strip, followed by img_2.png, and the pixel data in img_1.png is directly succeeded by that in img_2.png during concatenation. Figure 1.1 provides a visual representation of this concatenation order. To address this challenge, a tool named findpng is created to search the directory hierarchy for authentic PNG files. Additionally, a concatenation tool named catpng is developed to merge pixel data from a set of PNG files into a single PNG image file, with the constraint that all PNG images must share the same width dimension.

PNG Concatentation:
The cat_png function will concatentate the PNG strips sequentially into one fully image. Five strips of images is shown below: \
![pic_cropped_0](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/346bbe3b-fdc9-451b-bdba-f8274ba44c4f) \
![pic_cropped_1](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/0e2d8110-5d37-4800-ae64-991ccb57dab2) \
![pic_cropped_2](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/5294b576-eedc-4118-8383-54917f967647) \
![pic_cropped_3](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/8c4550d3-743f-4b5b-879b-cece36864cc9) \
![pic_cropped_4](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/82be959e-bc68-4335-b37f-adff769abaad) 

After feeding the five images into the program with the following command in terminal: ./a.out img1.png img2.png img3.png img4.png img5.png
The following image will be generated as "all.png" as shown: \
![WEEF_1](https://github.com/Max00358/PNG_Finding_and_Concatentation/assets/125518862/483b5d2d-3d83-4dbb-9902-8da949c360af)
