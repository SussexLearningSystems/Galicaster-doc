
Hauppauge device module
=======================
**NOT TESTED WITH GALICASTER 2**
**THIS PAGE IS UNDER CONSTRUCTION**

The Hauppauge module is adapted to take advantage of the features of hardware encoding Hauppauge cards. These cards encode both audio and video into a MPEG2 stream.

### Module Compatibility
* [Hauppauge capture cards](Devices/Hauppauge.md)  
  *  Hauppauge PVR-350  
  *  Hauppauge PVR-250  
  *  Hauppauge PVR-1600  

### Plugin configuration
Admitted values:

* `name`: Name assigned to the device.
* `device`: Device type: hauppauge
* `flavor`: Matterhorn "flavor" associated to the track. (`presenter`|`presentation`|`other`)
* `location`: Device's mount point of the MPEG output.
* `locprevideo`: Device's mount point of the RAW output.
* `locpreaudio`: Device's mount point of the PCM output.
* `file`: The file name where the track will be recorded.
* `vumeter`: Whether the audio input would be represented on the vumeter. (`True`|`False`)
* `player`: Whether the audio input would be played on preview. (`True`|`False`)

### Examples:
```ini
[track1]
name = Hauppauge
device = hauppauge
flavor = presenter
location = /dev/haucamera
locpreavideo = /dev/hauprevideo
locpreaudio = /dev/haupreaudio
file = CAMERA.mpg
vumeter = True
player = True
```
