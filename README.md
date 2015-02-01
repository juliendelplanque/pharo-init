# pharo-init
A little bash script to initialize a directory so it's ready to work with pharo.

I'm planning to create a script to download images and put them in the right directory
in the image's stock.

## Organisation

Images are stocked in $HOME/.pharo/imgs by default. In this directory there are directories
named by numbers. These numbers represent the image version (3 for pharo3, 4 for pharo4, etc...).
Each directory may contain directories that contains image file and source file. These are named
according to the image version (for example: 30860 contains "Pharo-30860.changes" and  "Pharo-30860.image").

The source file is stocked in $HOME/.pharo/sources.

## How to use
A typic use would be:
~~~
$ pharo-init myproject -v 3 -i 30860
~~~

Or simply:
~~~
$ pharo-init myproject
~~~
if you want to use the latest image of pharo3.
