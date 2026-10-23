# Fold Camera

> **Source publication status:** Repository setup is complete. The full v143.3.3 source tree, including the bundled portrait models, is pending its initial Git push. Please do not treat this documentation-only state as a buildable checkout.

Fold Camera is an independent Android camera application based on [GrapheneOS Camera](https://github.com/GrapheneOS/Camera). **It is not an official GrapheneOS project and is not endorsed by GrapheneOS.**

## Features

- Photography, video recording, QR scanning, front and rear cameras
- Portrait mode with locally bundled depth and segmentation models
- Horizontal **180° and 360° panoramas**
- **Dual Photo and Dual Video** with picture-in-picture and split-screen layouts
- Manual camera controls, burst, slow motion, hyperlapse and interval capture
- Customizable camera mode strip and foldable-device support

Dual Photo combines the preview streams into a JPEG; its maximum resolution is limited by preview resolution. Photos are stored in `DCIM/Dual Photo`, and dual recordings in `DCIM/Dual Video`. Dual Photo also offers torch and screen-based illumination where supported.

Some dual-camera functionality uses a CameraX prerelease and may depend on device capabilities.

## Building from source

After the complete source is committed, install **JDK 21** and the Android SDK, then run:

```sh
printf 'sdk.dir=%s\n' "${ANDROID_HOME:-$HOME/Android/Sdk}" > local.properties
./gradlew :app:assembleDebug --no-daemon
```

For local release builds on Arch Linux, see `BUILD_ARCH.sh`. Signing keys are **not** part of the repository.

Run `python3 tools/check-source-hygiene.py` and `./gradlew :app:lintRelease --no-daemon --console=plain` to verify the source. Test camera behavior on target hardware.

## APK releases

Source releases and installable APKs are different artifacts. A signed APK may be attached separately under [Releases](../../releases) later.

## Upstream and licenses

This is a third-party derivative of GrapheneOS Camera. Retain the original [MIT license](LICENSE), source copyright notices and all notices for third-party components and bundled ONNX models. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for details.
