Plex New Transcoder Unofficial Source Repository README
=======================================================

This is the source pulled from [Plex](http://www.plex.tv/) for the Plex Media Server (closed
source application).  The repository was generated by downloading the original transcoder
(Plex Transcoder), included in the current build with source located at http://files.plexapp.com/elan/ffmpeg/PlexTranscoder.tar.bz2

After downloading, I committed and grabbed the Plex New Transcoder at http://files.plexapp.com/elan/ffmpeg/PlexNewTranscoder.tar.bz2
and overwrote the transcoder to allow a somewhat reasonable diff between the versions. Much of the code is simply FFmpeg and the
original readme is provided below.

I will attempt to keep this updated.  The text below will indicate the download time, however, always check those above links (or 
whatever links are referenced in the LICENSE file included with Plex Media Server). I will always update the readme when
a new version is downloaded.

Version Represented by this Repository
======================================

The PlexTranscoder and PlexNewTranscoder represented by this repository were downloaded from the above links on 30 May 2015 at 
about 11:00 PM Eastern Daylight Time

Why are you doing this?
=======================

At the present time Plex does not publish this code to their git repository. This is inconvenient (and disappointing). I'm
interested in experimenting with the transcoder and FFmpeg has been a project I've loved to tinker with. There are many
unofficial patches for FFmpeg that I'd like to experiment with.  But mostly becuase "it was there."

I'll write a script to keep this up-to-date with the vanilla sources released by Plex and I'll publish that script once I
take some of my (limited) personal time to write it. For now, always check the links above to make sure you're current.

Limitations
===========

Presently, it appears two important files are missing, plexConfig.h and plexVersion.h.  I have not attempted to make/compile
this, yet. I'm not expecting good results.  I'll be following up with the Plex and FFmpeg folks to see about resolving this
problem (I believe failing to include these files may be in violation of the LGPL-licensed FFmpeg).  Hopefully that gets
solved!

Otherwise, consider this little more than an academic exercise.

FFmpeg README
=============

FFmpeg is a collection of libraries and tools to process multimedia content
such as audio, video, subtitles and related metadata.

## Libraries

* `libavcodec` provides implementation of a wider range of codecs.
* `libavformat` implements streaming protocols, container formats and basic I/O access.
* `libavutil` includes hashers, decompressors and miscellaneous utility functions.
* `libavfilter` provides a mean to alter decoded Audio and Video through chain of filters.
* `libavdevice` provides an abstraction to access capture and playback devices.
* `libswresample` implements audio mixing and resampling routines.
* `libswscale` implements color conversion and scaling routines.

## Tools

* [ffmpeg](http://ffmpeg.org/ffmpeg.html) is a command line toolbox to
  manipulate, convert and stream multimedia content.
* [ffplay](http://ffmpeg.org/ffplay.html) is a minimalistic multimedia player.
* [ffprobe](http://ffmpeg.org/ffprobe.html) is a simple analisys tool to inspect
  multimedia content.
* Additional small tools such as `aviocat`, `ismindex` and `qt-faststart`.

## Documentation

The offline documentation is available in the **doc/** directory.

The online documentation is available in the main [website](http://ffmpeg.org)
and in the [wiki](http://trac.ffmpeg.org).

### Examples

Coding examples are available in the **doc/examples** directory.

## License

FFmpeg codebase is mainly LGPL-licensed with optional components licensed under
GPL. Please refer to the LICENSE file for detailed information.
