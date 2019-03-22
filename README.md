# slides_with_video
Example of slides with video to test PDF viewers such as okular and evince. See also Bug [#1821298](https://bugs.launchpad.net/ubuntu/+source/evince/+bug/1821298) on Launchpad.

## Compile with:
```pdflatex slides_with_video```

The resulting PDF file is included in the repository to allow testing without a LaTeX distribution

## Expected behaviour
Both in normal and presentation mode, the video should
* play when clicking
* stop when changing slide and the video frame should disappear

## Evince (version 3.28.4 on Ubuntu 18.04)
In normal mode:
* the video contines playing and the video frame covers the content of the next slides

In presentation mode:
* the video does not play at all
