# Evolcon Widget Library
This is a widget library developed by Evolcon (well... duh...). It contains several objects

## Getting Started

#### Qlik Sense Dektop
1. Download the package and unzip it.
2. Copy the new folder to this location: C:/Users/?????/Documents/Qlik/Sense/Extensions/.

#### Qlik Sense Server
Although widget libraries can be imported from both QMC and Dev Hub, the uniqueness check of a widget is only performed when importing from Dev Hub. Therefore, we strongly recommended you import all widget libraries from Dev Hub.
1. Download the ZIP file.
2. Open the Qlik Dev Hub. On the start page, click **+** and select **Import widget library**.
3. Locate the ZIP file containing the widget library to import and then click **Open**.

#### Demo App
Don't forget to check the demo app included in this package. It contains some examples of all the widgets in the library.

## QlikFreak KPI
Simple KPI with an image on the left.
<p align="center"><img src="https://qlikfreak.files.wordpress.com/2018/02/35_1001.png"></p>
This widget only receives one expression and it has 4 blocks:

* **Image**: Link to the image file (JPG, PNG, SVG, etc).
* **Title:** First line. Usually displays the KPI name, but it can be hidden.
* **KPI:** Big number in the middle (your expression).
* **Comment:** Third line. Useful for comments of comparisons. Can be hidden as well.

### Notes

* When you define the width of the image, the height is calculated automatically.
* **Right Padding** refers to the distance (pixels) between the image and the numbers.
* All the labels can be static (just type in whatever you want) or dynamic (using Qlik expressions) 
```
='Amount (USD): ' & money(sum(Sales))
```
* You can use RGB, HEX or [CSS colors](https://www.w3schools.com/cssref/css_colors.asp). If the color is static, you can type it directly in the box:
```
rgb(100, 50, 10)
turquoise
#FFF000
```
If you want to use an expression, you can do something like this:
```
=if(sum(Sales) > 1000, rgb(255, 50, 10), 
 if(sum(Sales) > 500, 'turquoise', '#FFF000'))

```

## Authors
* **Evolcon** [Visit Website](http://evolcon.com/)
* **Julian Villafuerte:** [QlikFreak](https://qlikfreak.wordpress.com/)  -  [Twitter](https://twitter.com/qlikfreak)


