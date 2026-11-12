# BuntyTune

BuntyTune is an original JUCE-based vocal pitch-correction and enhancement plugin. The plugin interface includes the user-provided studio portrait embedded as a build resource.

## Included features

- Auto Key Pitch Correction (automatic key estimation mode, plus manual key/scale selection)
- Retune Speed
- Natural Voice (vibrato/expression preservation)
- Compressor (threshold, ratio, attack, release, makeup gain)
- Vocal Enhance (low cut, presence, air, output gain)
- Custom studio portrait in the plugin header (embedded; no external image file needed at runtime)

## Build on Windows

This project uses JUCE 8.0.4 and CMake. Open the repository on GitHub and run **Actions → Build BuntyTune (Windows x64) → Run workflow**. The workflow uploads the build output as the `BuntyTune-Windows-x64` artifact.

## Plugin format note

This JUCE 8 project is configured to build **VST3** and **Standalone**. It does not produce a legacy VST2 `.dll`. A VST2 build requires a compatible legacy JUCE setup and the appropriate Steinberg VST2 SDK/licensing. Cubase supports VST3; install the resulting `.vst3` plugin in the system VST3 folder.
