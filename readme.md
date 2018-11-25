# GPMDP widget for OBS
Google Play Music Desktop Player widget for Open Broadcaster Software.

It shows current song information on your stream.

Format:
```
Song Title
Song Artist — Song Album
```

## Setup
1. Enable JSON API in GPMDP (Desktop Settings → General → Enable JSON API).

2. Create symlink of `playback.json` in the directory of `playback.html`. Locations for different systems are described [here](https://github.com/MarshallOfSound/Google-Play-Music-Desktop-Player-UNOFFICIAL-/blob/master/docs/PlaybackAPI.md). It must be something like this:

    Linux:
    ```bash
    ln -s playback.json ~/.config/Google Play Music Desktop Player/json_store/playback.json
    ``` 

    Windows:
    ```
    mklink /d playback.json %APPDATA%\Google Play Music Desktop Player\json_store\playback.json 
    ```

    MacOS:
    ```bash
    ln -s playback.json ~/Library/Application Support/Google Play Music Desktop Player/json_store/playback.json
    ``` 

3. Add Browser source to your OBS, and point the local `playback.html` file.
