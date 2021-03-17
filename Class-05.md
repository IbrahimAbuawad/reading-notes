## HTML
### Images
#### The **img** element is used to add images to a web page .
#### You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
##### Example :
`<img src="url of image"/>`
#### You should save images at the size you will be using them on the web page and in the appropriate format.
#### X Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.
#### When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.
#### we can change width and height of image . 
##### Example :
###### img src="images/quokka.jpg" alt="A family of quokka" width="600" height="450"


### Color 
#### Color not only brings your site to life, but also helps convey the mood and evokes reactions .
#### There are three ways to specify colors in CSS:
##### 1. RGB values .
##### 2. hex codes .
##### 3. color names .

#### Color pickers can help you find the color you want.
#### CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
#### CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


### Text
#### There are properties to control the choice of font, size, weight, style, and spacing.
`font-size : 20px ; font-weight: bold ;`
#### There is a limited choice of fonts that you can assume most people will have installed.
##### Examples of fonts :
###### Georgia , Times , Times New Roman , Sans-Serif , Sans-serif 


#### If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.

#### You can control the space between lines of text, individual letters, and words. Text can also be aligned to the 
##### 1. left 
##### 2. right 
##### 3. center
##### 4. justified

#### You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

![Font property](https://jobs.sapcanvas.com/wp-content/uploads/2020/10/fig7-CSS-Text-Properties-1024x429.png)


## JPEG vs PNG vs GIF
#### Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.
#### Compression can be of two types :
##### 1. lossless : it is possible to reconstruct the original image from the compressed image because there is no information loss during compression.
##### 2. lossy : this compression ratio comes at a cost of reduced quality that becomes more evident after zooming in on the image. 

*JPEG is a lossy compression specification*
*PNG is a lossless image format using DEFLATE compression.*
*GIF is also a lossless image format that uses LZW compression algorithm.*

#### Transparency : transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours.

*JPEG images don’t support transparency and are hence not usable for such cases.*
*GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency).*

#### PNG images support transparency in two ways :
##### 1. inserting an alpha channel that allows partial transparency
##### 2. by declaring a single colour as transparent (index transparency).

#### Animations refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video.