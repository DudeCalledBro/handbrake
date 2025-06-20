# HandBrake

This repository contains my scripts for transcoding DVDs and Blu-rays for Jellyfin, using HandBrake and HandBrakeCLI.

## Setup

Installing on macOS with Homebrew is straightforward. First, install HandBrake:

```bash
brew install --cask handbrake
```

Next, download the HandBrakeCLI `.dmg` file from the HandBrake GitHub Releases ([here](https://github.com/HandBrake/HandBrake/releases)). Make sure you download the version that matches your HandBrake installation:

```bash
sudo cp /Volumes/HandBrakeCLI-1.9.1/HandBrakeCLI /usr/local/bin/
```

## Transcoding

You dont have to use the provided transcode script to run HandBrake, but we value efficiency! Plus, I prefer not to manually configure encoding settings every time, even with templates. So just fire up the script!

```bash
# Make the script executable
chmod +x transcode.sh

# Transcode your Blu-ray disc
./transcode.sh ~/Desktop/Jason Bourne
```

## License

Copyright © 2025 Niclas Spreng

Licensed under the [MIT license](LICENSE).
