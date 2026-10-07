DISCLAIMER: This program is free software: you can redistribute it and/or 
modify it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or (at your option) 
any later version. This program comes with ABSOLUTELY NO WARRANTY, 
to the extent permitted by law. The full license is featured in the source folder
and the "ffmpeg" folder as LICENSE.txt.

Copyright (C) 2026 Archie Garlick-Freeston

Thanks for downloading convertBud. This was a simple tool I made 
with help from AI for myself so that FFmpeg was easy for me to use.

Most usage instructions are provided directly in the program, 
so this README mainly provides additional information.

> What is convertBud?

convertBud is a command-line file converter based on an FFmpeg build
from https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-essentials.zip. 
It's made to be simple and easy to use, like an FFmpeg "lite" app.

It is completely free and open source, and comes with a copy of 
FFmpeg essentials. Feel free to do what you'd like to convertBud
under the GNU license.

> What can convertBud do?

File conversion:

- Image to image (batch and single conversion)
Example: .JPG to .PNG
- Audio to audio and video (batch and single conversion)
Example: .WAV to .MP3, .WAV to .MP4
- Text files
Note: Only changes the type, not the content of the file.
This may cause errors outside of convertBud, even if it does
successfully convert.

The tool is built to look clean. FFmpeg's source output is silenced,
obviously barring important information like errors. Existing output files 
are never overwritten.

> What are the prerequisites around convertBud?

- A Windows operating system, best bet is Win10 onwards. See FFmpeg's
requirements too.
- The included FFmpeg Essentials build.
- The FFmpeg executable (convertBud\ffmpeg\bin\ffmpeg.exe is the
expected directory).

That's it, as far as I'm aware.

> How do I use convertBud?

Double-click or open convertBud.bat - an options menu should appear,
then follow the instructions in the command line, there are plenty.

The input folder includes files to convert. Drag your files into here
and convertBud can read them. The output folder is where converted
files live after a successful conversion. Use this folder to store 
cover images for your audio to .mp4 conversions.

> What are convertBud's limitations?

Some of these are subject to change.

- Text conversion cannot translate formats.
- MP4 output is only 1920x1080.
- WAV output has a locked bit depth.
- Not every possible FFmpeg format is exposed by convertBud.

> Extras:

- convertBud is not affiliated with FFmpeg. FFmpeg is a separate project, 
and convertBud is, again, not affiliated with the FFmpeg project.

- Currently available conversion formats:

Audio:	 WAV, MP3, FLAC, M4A, AAC, OGG, MP4.
Images:	 JPG, JPEG, PNG, BMP, WEBP, GIF, TIF, TIFF.
Text:    Choose your own extension.

- The output file keeps the input filename, so if you converted Sound.mp3
to the .wav, it'd be Sound.wav. Spaces are supported, so Sound Effect.mp3
would be just as viable as SoundEffect.mp3.

- A few things about batch conversion:

> Files are only read from the input directory.
> Batch conversion only supports file conversion that single conversion
of the same filetype supports. Unsupported files are ignored.
> 50 files is the vanilla maximum amount for a batch conversion.
This can be changed, but do so at your PC's risk.



