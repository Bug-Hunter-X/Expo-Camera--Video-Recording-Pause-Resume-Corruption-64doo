# Expo Camera Video Recording Pause/Resume Bug

This repository demonstrates a bug in Expo's Camera API related to pausing and resuming video recording.  When attempting to manually pause and resume video recording using the `recordAsync` method, the resulting video may be corrupted or recording might stop unexpectedly without any error messages in the console.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Try to record a video. Pause recording and then resume it multiple times. 
5. The recorded video may be corrupted or stop unexpectedly. 

## Solution

The provided solution demonstrates one potential workaround. The approach involves checking the camera status after resuming recording to ensure it's properly recording and handling potential errors gracefully. Further investigation and a potential fix might require deeper inspection of the Expo Camera API's internal handling of asynchronous recording operations.
