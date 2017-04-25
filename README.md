# React Native Exif 
An image exif reader updated on iOS for use with the Photo Framework - instead of AssetsLibrary

## Installation
```sh
npm install francisco-sanchez-molina/react-native-exif --save
rnpm link react-native-exif
```


## Usage

```javascript
import Exif from 'react-native-exif'

....

Exif.getExif('/sdcard/tt.jpg')
    .then(msg => console.warn('OK: ' + JSON.stringify(msg)))
    .catch(msg => console.warn('ERROR: ' + msg))

...

Exif.getExif('content://media/external/images/media/111')
    .then(msg => console.warn('OK: ' + JSON.stringify(msg)))
    .catch(msg => console.warn('ERROR: ' + msg))

...

Exif.getExif('assets-library://asset/asset.JPG?id=xxxx&ext=JPG')
    .then(msg => console.warn('OK: ' + JSON.stringify(msg)))
    .catch(msg => console.warn('ERROR: ' + msg))

```
### Exif values

Value | 
--- |
ImageWidth |
ImageHeight |
Orientation |
originalUri |
exif|


Version 0.1.0 add react-native 0.40 support
