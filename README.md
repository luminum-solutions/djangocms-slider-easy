djangocms-slider
================

A simple django cms slideshow plugin. For of https://github.com/urga/djangocms-slider, but using easy-thumbnails by default.

Features:

* There are 2 plugins: SlideShow and Slide. A SlideShow can only contains Slides. Those can be arranged in the order you want just like any other plugin.
* Each image can have a url specified (creating an anchor around the image)
* By default, creates a [flexslider](http://www.woothemes.com/flexslider/) slideshow.
* By default, uses [easy-thumbnails](https://github.com/SmileyChris/easy-thumbnails) as a thumbnail plugin.

Installation
------------

This plugin requires `django CMS 3.0` or higher to be properly installed and configured.

To install:

* run `pip install djangocms-slider-easy` on your virtualenv
* add `easy_thumbnails` to your `INSTALLED_APPS` setting if you want to use default template.
* add `djangocms_slider` to your `INSTALLED_APPS` setting (mind the underscore)
* Run `./manage.py migrate djangocms_slider`

Usage
-----

To override the template, just add `slider.html` and or 'slide.html' in a django template directory under `templates/djangocms_slider`.
