# video_player_rtmp_ext
[![pub](https://badgen.net/pub/v/video_player_rtmp_ext)](https://pub.dev/packages/video_player_rtmp_ext)
A player supporting rtmp&rtmps live video

## Getting Started

```yaml
video_player_rtmp_ext: ^last_version
```

## 1.Simple example

* Initialize controller

```dart
IJKPlayerController controller = IJKPlayerController.network("http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8");
```

* Using widgets

```dart
VideoPlayerRtmpExtWidget(
   controller: controller,
   viewCreated: (IJKPlayerController _){
       controller.play();
   },
)
```

## 2. Controller API

* Start playing
```dart
controller.play();
```
