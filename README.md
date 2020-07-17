# gran
Basic and fully customizable Open edX theme

This theme is an combinations of  https://github.com/overhangio/indigo  and https://github.com/dehamzah/starter-theme-openedx
 
 It's very basic but  powerful, you can change most part of LMS very easily. I tired this on Tutor(https://docs.tutor.overhang.io/) which is Open edx Juniper(https://open.edx.org/).But that can be implement native version of Juniper as well.

 ## Installation:

 Clone this repository:

 ` git clone https://github.com/murat-polat/gran`

 Render (paver/update) theme:

  `tutor config render  ./gran/theme "$(tutor config printroot)/env/build/openedx/themes/gran" `

Rebuild the Open edX docker image::

tutor images build openedx


Restart your platform::


tutor local quickstart   or ` tutor local start -d`


Set your theme some default theme:

tutor local settheme gran localhost  $(tutor config printvalue LMS_HOST) 




Done :)

![](src/head.png)
![](src/foot.png)