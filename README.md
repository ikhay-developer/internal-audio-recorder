# Internal Audio Recorder Flutter Plugin

Flutter plugin for capturing internal audio on Android devices.

## Installation

Add the following to your `pubspec.yaml` file:

```yaml
dependencies:
  internal_audio_recorder: ^1.0.0
```

## Usage

import 'package:internal_audio_recorder/internal_audio_recorder.dart';

```yaml
// Example usage void startRecording() async { String result = await
InternalAudioRecorder.startCapturing(
outputPath: "path/to/output/file", encoding: InternalAudioRecorder.ENCODING_PCM_16BIT, sampleRate:
44100,
); print(result); // Output: "Recording started" or an error message }

void stopRecording() { InternalAudioRecorder.stopCapturing(); print("Recording stopped"); }
```
API Reference InternalAudioRecorder.startCapturing Starts capturing internal audio.

Parameters outputPath (String): The path to the output file. encoding (int): The audio encoding
format (e.g., InternalAudioRecorder.ENCODING_PCM_16BIT). sampleRate (int): The audio sample rate.
Returns A String indicating the result of the operation.

InternalAudioRecorder.stopCapturing Stops the audio capturing process.

