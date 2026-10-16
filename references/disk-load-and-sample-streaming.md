# Disk Load And Sample Streaming

Open when you need guidance on Disk Load And Sample Streaming in Ableton Live.

Context: [Computer Audio Resources and Strategies](computer-audio-resources-and-strategies.md#37-computer-audio-resources-and-strategies).

<a id="source-372-managing-the-disk-load"></a>
### 37.2 Managing the Disk Load

How quickly an SSD reads and writes has a bearing on how Live performs. The volume of disk traffic Live creates scales more or less with how many audio channels are being read or written at the same time. To take one case, a track sounding a stereo sample drives more disk traffic than one sounding a mono sample.

The Disk Overload Indicator.

Whenever the disk fails to read or write audio fast enough, the Disk Overload indicator blinks. While you're recording, that situation leaves a gap in the captured sample; during playback, it surfaces as dropouts.

To steer clear of disk overload, try these steps:

- Cut how many audio channels you write by picking mono inputs over stereo inputs within the Audio Settings’ Channel Configuration dialog.
- Switch on [RAM Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-ram-mode) for the clips you choose.
- Lower the count of audio channels in playback by favoring mono samples over stereo samples wherever you can. Turning a stereo sample into mono is doable in any ordinary digital audio editor, which you can launch [from within Live](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#viewing-and-changing-a-live-sets-file-references).
