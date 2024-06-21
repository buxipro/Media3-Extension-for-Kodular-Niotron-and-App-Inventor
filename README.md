## Media Player Extension based on Androidx Media3 Library for AppInventor, Kodular and Niotron, Media3 is upgraded version of Exoplayer

Hello dear! it's **Media Player Extension based on Androidx Media3 Library** in this extension i used Androidx Media3 library **version 1.3.1** it's latest version of Media3. Why i not used **Exoplayer library** to create this extension because Exoplayer is deprecated and google will not continue exoplayer because **Google launched Media3, Media3 contains all exciting Exoplayer features and even more** basically **Media3** is upgraded version of **Exoplayer**.
Our extension support all Media protocols like MP4, HLS, DASH, RTSP and SmoothStreaming. This Extension will be best choice for **Developers** who demand the best performance and flexibility in media.

## Feature's

✔️ **Support all DRM protected media's.**   

✔️ **Most highlighted feature is developer can create custom controls, Any type he/she want..**   

✔️ **Default Controls.**

![DefaultControls](images/Default_Controls.png)

✔️ **Custom Controls**   

![CustomControls](images/Custom_Controls.png)

✔️ **Quality selection, user can change quality.** 

![QualitySelection](images/TracksScreenshot.png)


# Supported formats

✔️ Streaming: HLS, DASH, RTSP and SmoothStreaming  
✔️ Containers: MP4, MOV, FLV, MKV, WebM, Ogg, MPEG  
✔️ Video: H.263, H.264 AVC, H.265 HEVC, MPEG-4 SP, VP8, VP9, AV1  
✔️ Audio: Vorbis, Opus, FLAC, ALAC, MP1, MP2, MP3, AAC, AC-3, E-AC-3, DTS, DTS-HD, TrueHD

# DRM

✔️ Widevine  
✔️ Clearkey  
✔️ Playready

# Events

### OnAudioSessionIdChanged

![OnAudioSessionIdChanged](images/OnAudioSessionIdChanged.png)

**Event raised when audio session change.**

audioSessionId = **Number**

### OnControlsVisibilityChanged

![OnAudioSessionIdChanged](images/OnControlsVisibilityChanged.png)

**Event raised when controls visible or hide.**

visible = **Boolean**

### OnCues

![OnCues](images/OnCues.png)

**Event raised when **Text** output changes.**

cues = **List**

### OnFullscreenButtonClick

![OnFullscreenButtonClick](images/OnFullscreenButtonClick.png)

**Event raised when fullscreen button clicked.**

isFullscreen = **Boolean**

### OnIsLoadingChanged

![OnIsLoadingChanged](images/OnIsLoadingChanged.png)

**Event raised when the player starts or stops loading.**

isLoading = **Boolean**

### OnIsPlayingChanged

![OnIsPlayingChanged](images/OnIsPlayingChanged.png)

**Event raised when the player's play/pause state changes.**

isPlaying = **Boolean**

### OnMaxSeekToPreviousPositionChanged

![OnMaxSeekToPreviousPositionChanged](images/OnMaxSeekToPreviousPositionChanged.png)

**Event raised when maximum seek to previous position change.**

maxSeekToPreviousPositionMs = **Number**

### OnMetadataChanged

![OnMetadataChanged](images/OnMetadataChanged.png)

**Event raised when media metadata changes.**

data = **Dictionary**

**Keys**

```
title,      
artist,     
albumTitle,    
albumArtist,     
displayTitle,   
subtitle,     
description,      
mediaType,     
artwork_uri,      
track_number,      
total_tracks,   
releaseYear,      
playable
```

### OnPlayWhenReadyChanged

![OnPlayWhenReadyChanged](images/OnPlayWhenReadyChanged.png)

**Event raised when play when ready change.**

playWhenReady = **Boolean**   
reason = **Number**

### OnPlaybackStateChanged

![OnPlaybackStateChanged](images/OnPlaybackStateChanged.png)

**Event raised when playback state has been changed.**

state = **Number**

### OnPlayerError

![OnPlayerError](images/OnPlayerError.png)

**Event raised when player got error.**

error = **Text**

### OnPositionDiscontinuity

![OnPositionDiscontinuity](images/OnPositionDiscontinuity.png)

**Event raised when position discontinuity.**

oldContentPositionMs = **Number**   
oldPositionMs = **Number**   
newContentPositionMs = **Number**   
newPositionMs = **Number**   

### OnProgressUpdate

![OnProgressUpdate](images/OnProgressUpdate.png)

**Event raised when progress update.**

positionMs = **Number**   
bufferedPositionMs = **Number**   
durationMs = **Number**   

### OnRenderedFirstFrame

![OnRenderedFirstFrame](images/OnRenderedFirstFrame.png)

**Event raised when video first frame rendered.**

### OnRepeatModeChanged

![OnRepeatModeChanged](images/OnRepeatModeChanged.png)

**Event raised when repeat mode change.**

repeatMode = **Text**

### OnSeekBackIncrementChanged

![OnSeekBackIncrementChanged](images/OnSeekBackIncrementChanged.png)

**Event raised when seek back imcrement change.**

seekBackIncrementMs = **Number** 

### OnSeekForwardIncrementChanged

![OnSeekForwardIncrementChanged](images/OnSeekForwardIncrementChanged.png)

**Event raised when seek forward imcrement change.**

seekForwardIncrementMs = **Number** 

### OnShuffleModeEnabledChanged

![OnShuffleModeEnabledChanged](images/OnShuffleModeEnabledChanged.png)

**Event raised when shuffle mode enabled change.**

shuffleModeEnabled = **Boolean** 

### OnTracksChanged

![OnTracksChanged](images/OnTracksChanged.png)

**Event raised when tracks changes.**

videoTracks = **List of Dictionary**   
audioTracks = **List of Dictionary**   
textTracks = **List of Dictionary**   

**Keys**

```
id,      
bitrate,     
accessibilityChannel,    
averageBitrate,     
channelCount,   
codecs,     
containerMimeType,      
cryptoType,     
frameRate,      
roleFlags,      
maxInputSize,   
width,      
height,     
language,       
label
```

### OnVolumeChanged

![OnVolumeChanged](images/OnVolumeChanged.png)

**Event raised when device volume change.**

volume = **Number**  
muted = **Boolean**  


# Functions

### CustomControls
**Add Custom controls layout in player view.**

![CustomControls](images/CustomControls.png)

**Required**    
controlsLayout = **Arrangement**    

### PlayerView
**Create a player view for player.**

![PlayerView](images/PlayerView.png)

**Required**    
playerLayout = **Arrangement**    
defaultControls = **Boolean** Set False if you set CustomControls

### MovePlayerView
**Move player view in another layout.**

![MovePlayerView](images/MovePlayerView.png)

**Required**    
newLayout = **Arrangement**    


### SetBufferingProgress
**Set Buffering Progress Layout.**

![SetBufferingProgress](images/SetBufferingProgress.png)

**Required**    
progressLayout = **Arrangement**    

**BufferingProgress**

![BufferingProgress](images/BufferingProgress.png)

### CreateTimeBar

![CreateTimeBar](images/CreateTimeBar.png)

**Required**    
layout = **Arrangement**    

**TimeBar**
![TimeBarSample](images/TimeBarSample.png)


### HideControls
**Hide the play view controls**

![HideControls](images/HideControls.png)

### ShowControls
**Show the play view controls**

![ShowControls](images/ShowControls.png)

### SetVolume
**Volume must be between device minimum volume to device maximum volume.**

![SetVolume](images/SetVolume.png)

**Required number**

### SetBrightness
**Brightness must be 0.1 to 1**

![SetBrightness](images/SetBrightness.png)

**Required number**


### Subbtitles sample

![Subtitles Sample](images/subtitles_demo.png)


## MediaItems

### DefaultMediaItem
**Create MediaItem for player.**

![DefaultMediaItem](images/DefaultMediaItem.png)

*Required**    
url = **Text**  
subtitles = **List**   

**Return MediaItem**

### MediaItem
**Create MediaItem for player with custom perameters.**

![MediaItem](images/MediaItem.png)

**Required**    
url = **Text**  
subtitles = **List**   
mimeType = **Text**   
mediaId = **Text**    
startPositionMs = **Number**  
endPositionMs = **Number**   
sartsAtKeyFrame = **Boolean**   
relativeToLiveWindow = **Boolean**   
relativeToDefaultPosition = **Boolean**   

**Default Values**

![MediaItemDefaultValues](images/MediaItemDefaultValues.png)

**Return MediaItem**

### AddMediaItem
**Add MediaItem in MediaItemList.**

![AddMediaItem](images/AddMediaItem.png)

**Required**    
index = **Number**  
**Set index 0 if want to add MediaItem at last in MediaItemList**  

mediaItem = **MediaItem**  

### SetMediaItemList

![SetMediaItemList](images/SetMediaItemList.png)

**Required List of MediaItems**

### GetMediaItemList
**Get MediaItem List you seted using SetMediaItemList/AddMediaItem.**

![GetMediaItemList](images/GetMediaItemList.png)

### RemoveMediaItems
**Remove MediaItems from MediaItemList.**

![RemoveMediaItems](images/RemoveMediaItems.png)

**Required**   
fromIndex = **Number**  
toIndex = **Number**   

### ClearMediaItemList
**Clear MediaItem List as you seted using SetMediaItemList/AddMediaItem.**

![ClearMediaItemList](images/ClearMediaItemList.png)

**MimeTypes**    

![MimeTypes](images/MimeTypes.png)

**Use DefaultMimeType if you didn't know MimeType.**

![DefaultMimeType](images/DefaultMimeType.png)

## MediaSoures

### HlsMediaSource
**Create HlsMediaSource for HLS playback.**

![HlsMediaSource](images/HlsMediaSource.png)

**Required**     
httpDataSource = **HttpDataSource**   
mediaItem = **MediaItem**   
allowChunklessPreparation = **Boolean**   
useSessionKeys = **Boolean**   
metadataType = **Number**  
timestampAdjusterInitializationTimeoutMs = **Number**   

**MetadataTypes**

![Metadatas](images/Metadatas.png)

**Default Values**

![HlsMediaSourceDefaultValues](images/HlsMediaSourceDefaultValues.png)

**Return MediaSource**

### RtspMediaSource

![RtspMediaSource](images/RtspMediaSource.png)

**Required**   
mediaItem = **MediaItem**  
userAgent = **Text**   
timeoutMs = **Number**   
debugLoggingEnabled = **Boolean**   
forceUseRtpTcp = **Boolean**   

**Default Values**

![RtspDefaultValues](images/RtspDefaultValues.png)

**Return MediaSource**

### SsMediaSource
**Create SsMediaSource for smooth streaming.**

![SsMediaSource](images/SsMediaSource.png)

**Required**    
httpDataSource = **HttpDataSource**   
mediaItem = **MediaItem**   
livePresentationDelayMs = **Number**   

**Default Value**

![LivePresentationDelayMs](images/LivePresentationDelayMs.png)

**Return MediaSource**

### DashMediaSource
**Create DashMediaSource for Dynamic Adaptive Streaming over HTTP (DASH) content.**

![DashMediaSource](images/DashMediaSource.png)

**Required**   
drmMedia = **DrmMedia**   
httpDataSource = **HttpDataSource**   
mediaItem = **MediaItem**   
fallbackTargetLiveOffsetMs = **Number**   
minLiveStartPositionUs = **Number**   

**Default Values**

![DashMediaSourceDefaultValues](images/DashMediaSourceDefaultValues.png)

**Return MediaSource**

### AddMediaSource
**Add AddMediaSource in MediaSourceList.**

![AddMediaSource](images/AddMediaSource.png)

**Required**    
index = **Number**  
**Set index 0 if want to add MediaSource at last in MediaSourceList**  

mediaSource = **MediaSource**  

### SetMediaSourceList

![SetMediaSourceList](images/SetMediaSourceList.png)

**Required List of MediaSources**

### GetMediaSourceList
**Get MediaSource List you seted using SetMediaSourceList/AddMediaSource.**

![GetMediaSourceList](images/GetMediaSourceList.png)

### RemoveMediaSources
**Remove MediaSources from MediaSourceList.**

![RemoveMediaSources](images/RemoveMediaSources.png)

**Required**    
fromIndex = **Number**  
toIndex = **Number**   

### ClearMediaSourceList
**Clear MediaSource List as you seted using SetMediaSourceList/AddMediaSource.**

![ClearMediaSourceList](images/ClearMediaSourceList.png)


## DrmMedia's

### DrmMedia 
**Create Drm Media for drm encrypted media. this fetch license keys from license url.**

![DrmMedia](images/DrmMedia.png)

**Required**   
drmScheme = **Text**   
licenseUrl = **Text**   
multiSession = **Boolean**   
forceDefaultLicenseUri = **Boolean**   
forceSessionsForAudioAndVideoTracks = **Boolean**   
playClearContentWithoutKey = **Boolean**   

**Return DrmMedia**

### LocalDrmMedia
**Create Drm Media with key id and key.**

![LocalDrmMedia](images/LocalDrmMedia.png)

**Required**   
drmScheme = **Text**   
keyId = **Text**   
key = **Text**   
inHex = **Boolean**   
multiSession = **Boolean**   
forceDefaultLicenseUri = **Boolean**   
forceSessionsForAudioAndVideoTracks = **Boolean**   
playClearContentWithoutKey = **Boolean**   

**Return DrmMedia**

**Default Values**

![DrmMediaDefaultValues](images/DrmMediaDefaultValues.png)

**Drm Scheme's**

![Schemes](images/Schemes.png)

### NoDrmMedia
**Use this if media doesn't required license.**

![NoDrmMedia](images/NoDrmMedia.png)


### HttpDataSource

![HttpDataSource](images/HttpDataSource.png)

**Required**    
allowCrossProtocolRedirects = **Boolean**   
connectTimeoutMs = **Number**   
keepPostFor302Redirects = **Boolean**   
readTimeoutMs = **Number**   
requestHeaders = **Dictionary**   
userAgent = **Text**   

**Default Values**

![HttpDataSourceDefaultValues](images/HttpDataSourceDefaultValues.png)

**Return HttpDataSource**

### Request Headers sample

![Request Headers Sample](images/demo_headers.png)

### SetHttpDataSource
**Use this only when you use just MediaItems not any MediaSources else this not work. If you're using MediaSources then you can set HttpDataSource directly in MediaSources..**

![SetHttpDataSource](images/SetHttpDataSource.png)

**Required**    
httpDataSource = **HttpDataSource**    


### ShowSpeedSelectionDialog

![ShowSpeedSelectionDialog](images/ShowSpeedSelectionDialog.png)

**Required**    
title = **Text**    

### ShowTrackSelectionDialog

![ShowTrackSelectionDialog](images/ShowTrackSelectionDialog.png)

**Required**    
title = **Text**    
trackType = **Number**    
showDisableOption = **Boolean**    
allowAdaptiveSelections = **Boolean**    
allowMultipleOverrides = **Boolean**    

### GetTracks
**Get Tracks of current playback content.**

![GetTracks](images/GetTracks.png)

**Required**    
trackType = **Number**    

**Return List of Dictionary**

### SelectTrack
**Select track from current tracks.**

![SelectTrack](images/SelectTrack.png)

**Required**    
trackType = **Number**    
index = **Number**    
**Set index 0 for Auto.**  

### TrackTypes

![TrackTypes](images/TrackTypes.png)

### SeekToPrevious

![SeekToPrevious](images/SeekToPrevious.png)

### SeekToNext

![SeekToNext](images/SeekToNext.png)

### SeekTo
**Seek to a specific position, set position in milliseconds.**

![SeekTo](images/SeekTo.png)

**Required**    
positionMs = **Number**    

### Rewind
**Set rewind milliseconds in properties mean how much they should rewind.**

![Rewind](images/Rewind.png)

### FastForward
**Set FastForward milliseconds in properties mean how much they should forward.**

![FastForward](images/FastForward.png)

### Prepare
**Call this before calling Play.**

![Prepare](images/Prepare.png)

### Play
**Call this after calling Prepare.**

![Play](images/Play.png)

### Pause
**Pause current player.**

![Pause](images/Pause.png)

### Resume
**Resume current player.**

![Resume](images/Resume.png)

### Stop 
**Stop current player.**

![Stop](images/Stop.png)

### Release 
**Release current player.**

![Release](images/Release.png)

### Destroy 
**Destroy current player, Note this reset all functions and properties before you called.**

![Destroy](images/Destroy.png)


### Format
**Format milliseconds to in time.**

![Format](images/Format.png)

**Required**    
ms = **Number**   


# Properties

### AutoHideControls
**Set controls will auto hide after timeout.**

![AutoHideControls](images/AutoHideControls.png)

**Required Boolean**

### AutoShowControls
**Set controls will auto show.**

![AutoShowControls](images/AutoShowControls.png)

**Required Boolean**

### BufferingColor
**Set center progress color.**

![BufferingColor](images/BufferingColor.png)

**Required Color**

### BufferedPercentage
**Return current BufferedPercentage in Number.**

![BufferedPercentage](images/BufferedPercentage.png)

### BufferedPosition
**Return current BufferedPosition in Number.**

![BufferedPosition](images/BufferedPosition.png)

### ControlsTimeout
**Set ControlsTimeout in milliseconds.**

![ControlsTimeout](images/ControlsTimeout.png)

**Required Number**

### CurrentBrightness
**Return current CurrentBrightness in Number.**

![CurrentBrightness](images/CurrentBrightness.png)

### CurrentMediaItemIndex
**Return current MediaItem/MediaSource index in Number.**

![CurrentMediaItemIndex](images/CurrentMediaItemIndex.png)

### CurrentPosition
**Return current playback position in Milliseconds (Number).**

![CurrentPosition](images/CurrentPosition.png)

### CurrentVolume
**Return current device volume in Number.**

![CurrentVolume](images/CurrentVolume.png)

### Customize TimeBar
**Required Color**

![TimebarColors](images/TimebarColors.png)

![Timebar_details](images/Timebar_details.png)

### FastForwardMs
**Set FastForward in milliseconds, How should forward after calling FastForward function.**

![FastForwardMs](images/FastForwardMs.png)

**Required Number**

### HasNext
**This return true if next MediaItem/MediaSource available, Return type Boolean.**

![HasNext](images/HasNext.png)

### HasPrevious
**This return true if previous MediaItem/MediaSource available, Return type Boolean.**

![HasPrevious](images/HasPrevious.png)

**Required Number**

### HideControlsOnTouch
**Set controls should hide on touch.**

![HideControlsOnTouch](images/HideControlsOnTouch.png)

**Required Boolean**

### IsControlsFullVisible
**This return true if controls visible, Return type Boolean.**

![IsControlsFullVisible](images/IsControlsFullVisible.png)

### IsSeekBackAvailable
**This return true if seek back/rewind available, Return type Boolean.**

![IsSeekBackAvailable](images/IsSeekBackAvailable.png)

### IsSeekForwardAvailable
**This return true if seek forward available, Return type Boolean.**

![IsSeekForwardAvailable](images/IsSeekForwardAvailable.png)

### KeepScreenOn
**Keep device screen always on.**

![KeepScreenOn](images/KeepScreenOn.png)

**Required Boolean**

### MaxVolume
**This return device maximum volume, Return type Number.**

![MaxVolume](images/MaxVolume.png)

### MinVolume
**This return device minimum volume, Return type Number.**

![MinVolume](images/MinVolume.png)

### PauseAtAndOfMediaItems
**Pause playback after each MediaItem/MediaSource.**

![PauseAtAndOfMediaItems](images/PauseAtAndOfMediaItems.png)

**Required Boolean**

### PlaybackSpeed
**Set playback speed, Which speed player should play.**

![PlaybackSpeed](images/PlaybackSpeed.png)

**Required Number**

### PlayWhenReady
**Set play when playback is ready.**

![PlayWhenReady](images/PlayWhenReady.png)

**Required Boolean**

### RepeatMode
**Set Repeat Mode.**

![RepeatMode](images/RepeatMode.png)

**Required**
### RepeatModes

![RepeatModes](images/RepeatModes.png)

### RewindMs
**Set Rewind in milliseconds, How should rewind after calling Rewind function.**

![RewindMS](images/RewindMS.png)

**Required Number**

### ResizeMode
**Set Resize Mode.**

![ResizeMode](images/ResizeMode.png)

**Required**
### ResizeModes

![ResizeModes](images/ResizeModes.png)

### ShowBuffering
**Set when buffering show.**

![ShowBuffering](images/ShowBuffering.png)

**Required**
![BufferingModes](images/BufferingModes.png)

## Buttons
**Set True if want to show else False.**

**Required Boolean**

### ShowFullscreenButton

![ShowFullscreenButton](images/ShowFullscreenButton.png)

### ShowNextButton

![ShowNextButton](images/ShowNextButton.png)

### ShowPreviousButton

![ShowPreviousButton](images/ShowPreviousButton.png)    

### ShowSettingsButton

![ShowSettingsButton](images/ShowSettingsButton.png)    

### ShowShuffleButton

![ShowShuffleButton](images/ShowShuffleButton.png)    

### ShowSubtitleButton

![ShowSubtitleButton](images/ShowSubtitleButton.png)    

### ShowVideoTracksButton

![ShowVideoTracksButton](images/ShowVideoTracksButton.png)    


### TotalBufferedDuration
**This return total buffered duration in milliseconds, Return type Number.**

![TotalBufferedDuration](images/TotalBufferedDuration.png)



## Extension specifications:
<b>Extension size:</b> 2.14MB\
<b>Extension Version:</b> 1.0.0\
<b>Media3 Library Version:</b> 1.3.1\
<b>Last amendment:</b> 11 June 2024\
<b>Demo Application:</b> <a href="https://github.com/buxipro/Media3-Extension-for-Kodular-Niotron-and-App-Inventor/raw/main/Media3.apk">Media3.apk</a> \
<b>Supported builder:</b> <a href="https://www.kodular.io/">Kodular</a>, <a href="https://niotron.com/">Niotron</a>, <a href="https://appzard.com/">AppZard</a>, <a href="https://androidbuilder.in/">AndroidBuilder</a>, <a href="http://ai2.appinventor.mit.edu/">App Inventor</a> and it's other distributions.\
<b>Extension price:</b> $10 (Pkr 3000)

## 📫 How to reach me ↓

<a href="https://wa.me/+923060335273" target="_blank">WhatsApp</a> | <a href="https://www.instagram.com/buxipro" target="_blank">Instagram</a></a>