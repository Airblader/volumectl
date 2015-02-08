# volumectl

`volumectl` is a small script that lets you control your sound volume, status and sink choice. This was only tested on my machine (Lenovo T530), so it might not work in all cases. It uses `pactl` and `pacmd` and basically serves as a convenience wrapper.

`sinkpicker` calls `volumectl` to list available sinks and pipes it into `dmenu`, the selected sink will then be used as the new default sink. This allows you to to choose between, e.g., headset and computer speakers. Any arguments given to it will be passed directly to `dmenu`. It expects `volumectl` to be in the path.
