# Comprehensive, custom Open edX Bootstrap theme,  gran-openedx-theme

Basic and fully customizable Open edX Bootstrap theme 

This theme is a combinations of  https://github.com/overhangio/indigo  and https://github.com/dehamzah/starter-theme-openedx
 
 It's  basic but  powerful. You can change most part of LMS very easily. I tired this on Tutor Juniper and Koa(https://docs.tutor.overhang.io/). But it's probably can work with native installations of Open edX also.

 ![](src/GranV3.gif)

 ## Installation:

 Clone this repository:

`$ git clone https://github.com/murat-polat/gran-openedx-theme`

 Render (paver/update) theme:

`$ tutor config render  ./gran-openedx-theme/theme "$(tutor config printroot)/env/build/openedx/themes/gran-openedx-theme" `

Rebuild the Open edX docker image:: ( For tutor production modus )

`$ tutor images build openedx`


Restart your platform::


`$ tutor local quickstart`   or  `$ tutor local start -d`


Set your theme some default theme:

`$ tutor local settheme gran-openedx-theme localhost studio.localhost  $(tutor config printvalue LMS_HOST) $(tutor config printvalue CMS_HOST)`



Note : After your code and customizations, you must repeat "render" , "build" and "quickstart" commands..

## Tutor development

https://docs.tutor.overhang.io/dev.html#customised-themes

`$ tutor dev runserver lms`

`$ tutor dev settheme gran-openedx-theme local.overhang.io:8000 studio.local.overhang.io:8001`

`$ tutor images build openedx-dev`

Start a new terminal than

`$ tutor dev run watchthemes`  For to compile your changes. 

Maybe you need an other terminal for "render" your customizations 

Done :)



