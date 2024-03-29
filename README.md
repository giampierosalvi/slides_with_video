# slides_with_video
Example of slides with video to test PDF viewers such as okular and evince. See also Bug [#1821298](https://bugs.launchpad.net/ubuntu/+source/evince/+bug/1821298) on Launchpad.

## Compile with:
```pdflatex slides_with_video```

The resulting PDF file is included in the repository to allow testing without a LaTeX distribution

## Expected behaviour
Both in normal and presentation mode, the video should
* play when clicking
* when changing slide the video should stop playing and the video frame should disappear

## Evince (version 3.28.4 on Ubuntu 18.04)
In normal mode:
* the video contines playing and the video frame covers the content of the next slides
* even if the video is stopped manually, the video frame does not disappear when changing slides

In presentation mode:
* the video does not play at all

## Okular (version 1.3.3 on Ubuntu 18.04)
Works as expected. It does not play the video in normal mode, but I suspect this is intended behaviour. Also it tends to crash with real presentations, but I have not been able to reporduce the crashes with this simple file.
