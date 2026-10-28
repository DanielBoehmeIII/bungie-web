# Third-party components

MediaPipe Tasks Vision 0.10.22-rc.20250304 is Apache-2.0 (see node_modules/@mediapipe/tasks-vision/package.json and https://github.com/google-ai-edge/mediapipe/blob/master/LICENSE). React is MIT; Lucide is ISC; Vite, Vitest and Playwright retain their package licenses.

The optional pretrained model assets are obtained directly from Google's official MediaPipe model storage at versioned URLs, listed with SHA-256 hashes in public/models/manifest.json. They are downloaded for local execution and excluded from the source repository. Model use follows the upstream terms and model cards linked from the official pages below. Do not infer that the code license automatically licenses every model weight; review upstream model terms before redistributing a packaged binary containing these assets.

https://developers.google.com/edge/mediapipe/solutions/vision/image_segmenter
https://developers.google.com/edge/mediapipe/solutions/vision/pose_landmarker
https://developers.google.com/edge/mediapipe/solutions/vision/gesture_recognizer

No copied TouchDesigner tutorial code or third-party portrait media is included. The demo is a locally drawn illustration.

## Desktop app

- softcam (https://github.com/tshino/softcam, MIT, incl. its MIT-licensed DirectShow base classes) is built into `bungie-camera.dll`, the Windows virtual camera, renamed to "Bungie"; its license ships next to the DLL as `bungie-camera-LICENSE.txt`.
- ONNX Runtime (MIT) is linked statically through the `ort` crate; OpenH264 (BSD-2-Clause) through `openh264`; other Rust crates are listed in `native/Cargo.lock` under their own licenses (MIT/Apache-2.0 and compatible).
- The installers bundle ONNX conversions of the MediaPipe models above; the same upstream model terms apply.
