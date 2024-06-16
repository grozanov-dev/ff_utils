Some helpful bash scripts to manipulate video with ffmpeg: encode, stabilize, play, etc...

# ff_264

Grades and encodes video to h264 for Youtube

Usage:
```
$ ./ff_264 <input_file> <lut_file> <output_file>
```
# ff_265_aac

Grades and encodes video to h265 with AAC audio for Youtube

Usage:
```
$ ./ff_265_aac <input_file> <lut_file> <output_file>
```
# ff_cut

Cut from timestemp

Usage:
```
$ ./ff_cut <input_file> <from_timestamp> <duration> <output_file>
```
Timestamp & duration format: HH:MM:SS

# ff_loudness

Detects true peak value from given audio

Usage:
```
    ./$ ff_loundess <audio_file> <seconds>
```
<seconds> - timestamp in format HH.MM.SS (ebur128 will detects clap in first hours, minutes and seconds of <audio_file>)

# ff_monitor

Plays video file with realtime timestamp

Usage:
```
$ ./ff_monitor <video_file>
```

# ff_peak_detection

Detects the offset of clap peak in audio

Usage:
```
    $ ff_peak_detection <audio_file> <seconds> <peak_value>
```
<seconds> - timestamp in format HH.MM.SS (ebur128 will detects clap in first hours, minutes and seconds of <audio_file>)

<peak_value> - value of true peak in dBTP (e.g. from ff_loudness)

# ff_prores_noaudio

Encodes video to ProRes LT 422 and removes audio track

Usage:
```
$ ./ff_prores_noaudio <input_file> <output_file>
```
# ff_sidebyside

Generates side-by-side comparison of two videos

Usage:
```
$ ./ff_sidebyside <video_1> <video_2>
```
# ff_stabilize

Stabilize video with VidStab lib, denoise and converts it to ProRes LT

Usage:
```
$ ./ff_stabilize <input_file> <output_file>
```
# ff_sync

Synchronize audio and video

Usage:
```
    ./ff_sync <audio_file> <shift_seconds> <video_file> <output_file>
```
# NOTE

You must get the release of ffmpeg built with VidStab

More info: https://gist.github.com/hlorand/e5012fa315dcfe358008cf1b4611c7e0

# Enjoy!

Sample video side-by-side: https://youtu.be/T4IV90zaD4E
