# Third-party notices — Fold Camera

Fold Camera is a third-party derivative of [GrapheneOS Camera](https://github.com/GrapheneOS/Camera), not an official GrapheneOS release.

The source archive includes the full notices and license copies below; they must be preserved when distributing the complete source.

## GrapheneOS Camera
Copyright GrapheneOS contributors. Original project under the MIT license; see [LICENSE](LICENSE).

## AndroidX ExifInterface fork
Derived from AndroidX ExifInterface 1.4.2 (Apache License 2.0), under `app/src/main/java/androidxc/exifinterface/`. Preserve original attribution.

## Portrait ONNX models
- [MODNet Photographic Portrait Matting](https://github.com/ZHKKKe/MODNet), distributed via [DavG25](https://huggingface.co/DavG25/modnet-pretrained-models), Apache 2.0. `modnet_photographic_portrait_matting.onnx` SHA-256: `07c308cf0fc7e6e8b2065a12ed7fc07e1de8febb7dc7839d7b7f15dd66584df9`.
- [Depth Anything V2 Small](https://github.com/DepthAnything/Depth-Anything-V2) via [ONNX Community](https://huggingface.co/onnx-community/depth-anything-v2-small), Apache 2.0. `depth_anything_v2_small_quantized.onnx` SHA-256: `fcf51f1b230362b28690bb9d1809bf0431f29cad20534e3f589bd7285547f20d`.

The pretrained weights are created by their respective upstream authors, not by Fold Camera.

## Libraries
- [ONNX Runtime](https://github.com/microsoft/onnxruntime): MIT
- AndroidX / CameraX: Apache 2.0
- [OpenCV 4.13.0](https://opencv.org/): Apache 2.0

## Panorama provenance
[Nokia AndroidOpenCameraKapture](https://github.com/nokia/AndroidOpenCameraKapture) and [Open Camera](https://sourceforge.net/p/opencamera/code/ci/master/tree/) were studied as references. No Nokia/Open Camera GPL implementation or RenderScript code is bundled; Fold Camera panorama code is an independent Kotlin implementation.

This is a summary only; the authoritative detailed notices and the Apache-2.0 license text are included in the complete v143.3.3 source archive.
