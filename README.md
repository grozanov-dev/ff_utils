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

# ff_monitor

Plays video file with realtime timestamp

Usage:
```
$ ./ff_monitor <video_file>
```
# ff_prores_noaudio

Encodes video to ProRes LT 422, denoise and removes audio track

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

Stabilize video with VidStab lib and converts it to ProRes LT

Usage:
```
$ ./ff_stabilize <input_file> <output_file>
```

# NOTE

You must get the release of ffmpeg built with VidStab

More info: https://gist.github.com/hlorand/e5012fa315dcfe358008cf1b4611c7e0

# Enjoy!

Sample video side-by-side: https://youtu.be/T4IV90zaD4E
