# SwiftuI_capture_recording_screenshot_event

```swift
        .onReceive(NotificationCenter.default.publisher(for: UIApplication.userDidTakeScreenshotNotification)) { _ in
            print("Screenshot taken")
        }
        .onReceive(NotificationCenter.default.publisher(for: UIScreen.capturedDidChangeNotification)) { _ in
            isRecordingScreen.toggle()
            print(isRecordingScreen ? "Started recording screen" : "Stopped recording screen")
        }

```
