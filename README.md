# movie2gif

Based on http://blog.pkh.me/p/21-high-quality-gif-with-ffmpeg.html

Copy the movie2gif to your bin folder and change its permissions to executable:

```
$ chmod +x movie2gif
```

The script uses the Linux readlink command. On Mac OS X this won't behave as expected. If that is the case, copy the readlink script to your bin folder and give it permissions to execute.

Alternatively you may clone the repository and create links to files in it:

```
$ ln -s $HOME/repos/external/movie2gif/movie2gif $HOME/bin/movie2gif
```

Run it without arguments to see the usage:

```
$ movie2gif 
> movie2gif <movie> [movie ...]
```

Run it with a movie file to create a file with the same name but in gif format:

```
$ ls -l
(...)
-rw-r--r--@ 1 eu  staff  2461868  3 Dec 09:37 movie.mov
$ movie2gif config.mov 
$ ls -l
(...)
-rw-r--r--  1 eu  staff  3228377  3 Dec 09:46 config.gif
-rw-r--r--@ 1 eu  staff  2461868  3 Dec 09:37 config.mov
```

## Dependencies

Depends on ffmpeg:

```
brew install ffmpeg
```
