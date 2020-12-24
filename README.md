# compton-tryone-transparency
My compton configuration for forced transparency

In order to use these effects make sure that you have installed `compton-tryone-git` from AUR and remove any other picom fork.

I have provided my comton configuration as an example. You can set opacity rules in this way-
```
active-opacity = 1.0;
frame-opacity = 0.7;
opacity-rule = [ "[Opacity 0-100]:class_g = 'window-name'"];
 ```
 Use xprop for the window name.
 Run `xprop |awk '/WM_CLASS/{print $4}'` and select the Window.
