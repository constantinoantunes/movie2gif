# movie2gif

Based on http://blog.pkh.me/p/21-high-quality-gif-with-ffmpeg.html

Copy the movie2gif to your bin folder and change its permissions to executable:

> chmod +x movie2gif

The script uses the Linux readlink command. On Mac OS X this won't behave as expected. If that is the case, copy the readlink script to your bin folder and give it permissions to execute.

Depends on ffmpeg:

> brew install ffmpeg
