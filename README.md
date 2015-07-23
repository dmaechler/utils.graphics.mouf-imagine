# Mouf Imagine

Mouf Imagine uses the [imagine/imagine](https://github.com/avalanche123/Imagine) library to create automated image transformations based on images' paths.

> A big thank to [Romain Neutron](https://github.com/romainneutron) for his great work, the quality of this library allowed us to integrate it in our framework with a few lines of code.

This is a module for the [Mouf PHP framework](http://mouf-php.com). In order to use this module, your code should also use [Splash, the MVC router for Mouf](http://mouf-php.com/packages/mouf/mvc.splash/index.md).

## The concept

<table style="width 100%; text-align: center">
<tr>
<th colspan="3">Let's say someone uploaded this image, But you need to display it in a smaller size, and in grayscale</th>
</tr>
<tr>
<td>
<img  width="300px"  src="doc/img/imagine.jpg" />
</td>
<td style="width: 20px;" align='center'> <font style="font-size: 60px">&#x21d2;</font> </td>
<td>
<img width="200px" src="doc/img/imagine-preset.jpg" />
</td>
</tr>
<tr>
<td> [WEB_ROOT]/uploads/image.jpg </td>
<td></td>
<td> [WEB_ROOT]/300x300_black_n_white/image.jpg </td>
</tr>
</table>

## How to ?

This is very simple ! All you have to do is create an instance of the `ImagePresetController` class :

<img width="80%" src="doc/img/simple-instance.png" />

In fact, what this package does for you is : apply a set of imagine filters on the original image, and display the image after saving it in the desired folder. All the rest is done by Imaging filters.


## Advanced features

We will try to get some optimisations in Imagine code (more explicit constructors, etc...) so it will eb easier to integrate that library in mouf. Moreover, for advanced image manipulation, please chekout the [utils.graphics.mouf-imagine-addons](https://github.com/thecodingmachine/utils.graphics.mouf-imagine-addons) package that will soon provide helpers and predefined advanced filters around the exising ones.

