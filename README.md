#musx
## introduce
musx is a free and open source audio playback library, based on OpenAL and libsndfile. Just add includes to your project and you're ready to go!
Author: Henry Du.
Last update: 2022/7/10
contact details:
(Domestic) 13552325266@163.com
(Foreign) wotsukoroga94@gmail.com
## UPDATE!!!
### MUSX v2.0.0 Update
Major update musx's programming style and API have been significantly updated!
Inspired by boost and the standard library, the musx namespace was re-lowercase,
Single file cancelled, now multiple hpp files.
musx switched to conan for dependency management, simplifying the build process.
---
#### New API:
1. oaudiostream: device and playback management.
2. isndstream : Audio file reading (mpeg format is not currently supported).
3. buffer_tool : Generate buffer, including two modes copy and extract.
4. source_manager: Manage audio elements.
5. streaming_manager: Manage music elements.
---
#### Deprecated
1. genAudioList and delAudioList, musx now focus more on core functionality.
2. The play and update_stream functions now use oaudiostream::operator<< for direct output.

## plan
1. MacOSX support.
2. More OpenAL features like alEffects...
3. Audio recording and file writing support.
4. mpeg format support.

## Construct
If you don't need a case, just copy all the contents in the include directory to your own project,
You need to install openal-soft and libsndfile by yourself.
### Build example
Just run build.sh/build.bat directly (you need to install python3 conan and cmake first)
## Documentation
The two examples in the examples folder are basically sufficient.
## Thanks to
Musx uses openal-soft and libsndfile; also, thanks to the free course on YouTube:
- **OpenAL-soft : https://github.com/kcat/openal-soft**
- **libsndfile : https://github.com/libsndfile/libsndfile**
- **YouTube Tutorial: https://www.youtube.com/watch?v=fG2veGWNPJY&list=PLalVdRk2RC6r7-4zciZ3LKc96ikviw6BS**
## License
musx uses the BSL license (boost-library-license) instead, which is taken from open source, back to open source, and pays homage to the standard library.

## Musx is made for games, its future belongs to a stronger game engine...
