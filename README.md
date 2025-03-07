# simplegp

SimpleGP is a module for interfacing with cameras using easy-to-understand and well-documented code using gphoto2 — the work of Marcus Meissner, et al., and Jim Easterbrook, who provide [libgphoto2/gphoto2](http://gphoto.org/) and the [gphoto2 bindings](https://github.com/jim-easterbrook/python-gphoto2) (respectively) — as the underlying engine.

The gphoto2 python module is a fantastic resource. Some coders, however — especially non-professionals and novices — may find it difficult to understand, utilize, or implement. SimpleGP will hopefully provide users a faster way to ramp up their projects by using familiar, camera-oriented language and plain english in its naming conventions, and doing the heavy lifting under the hood.

## MVP Functionality Goals
- Create a "camera" object that is connected to the physical camera
- Establish current camera's and lens's possible settings for ISO, Aperture, Shutter Speed, RAW/JPG capture
- Establish current configuration of aforementioned settings
- Enable modification of one of the aforementioned settings with value checking and guessing based on possible valid settings (e.g., if user tries to set aperture to 4, the module chooses 4.0. If user tries to set aperture to an invalid option, it will choose the nearest valid option from the list)
- Take photo, and decide whether to store the photo on the camera or the computer
- Unit testing with mocks

## Potential Future Goals
- Timelapse
- Focusing
