# Audio Sample File Formats

Open when you need guidance on Audio Sample File Formats in Ableton Live.

Context: [Managing Files and Sets](managing-files-and-sets.md#5-managing-files-and-sets).

<a id="source-51-sample-files"></a>
### 5.1 Sample Files

Any file holding audio data counts as a _sample_. Playback in Live covers uncompressed types (WAV, AIF and Sound Designer II for Mac) along with compressed ones (MP3, AAC, Ogg Vorbis, Ogg FLAC and FLAC).

Because samples stream straight off the disk during playback, even a hefty collection of sizeable samples won't bump up against your RAM ceiling. Be aware, though, that throughput trouble can surface when a drive sits almost full or (under Windows) is badly fragmented. The spin rate of a hard drive likewise plays a part in how well the disk performs. The section about [managing the disk load](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-disk-load) has further detail.

Uncompressed mono and stereo samples can be mixed together in Live regardless of their duration, sample rate or bit depth, and no conversion step is needed beforehand. When a compressed sample is involved, Live first decodes it and saves a temporary, uncompressed copy. The decode is generally fast enough that playback starts almost immediately, so there's no need to sit through the whole process.

Note: Should you bring a lengthy sample into a project, Live may warn that playback isn't possible until analysis has run. The [analysis](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#analysis-files-asd) section explains why.
