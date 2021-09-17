# BIDS youtube and podcast

## Requirements

Video editing done with [kdenlive](https://kdenlive.org/en/).

Post-montage sound levelling done with [Auphonic](https://auphonic.com/).

Edit right access to:

- the BIDS youtube channel
- the BIDS anchor podcast channel

## Inputs

- source video material stored on this
  [google drive](https://drive.google.com/drive/folders/1hQ3Ng5DJOOqYvFFinFAxoik-6NO5Xnkw?usp=sharing)
- "template" intro and outro slides are in the same folder

## Step by step

1. copy template and rename folder

TODO: Create template Github repo

1. rename `template.kdenlive` if this is for a youtube / posdacst episode:
   `episode-[episode number]\_title_here.kdenlive`

Add video place holder for new video

1. create / update intro slide from
   [these slides](https://docs.google.com/presentation/d/19-LQjDTDPXg0N8Z0LVH6ZyG0GaaiuactHIpuXTmPiQ8/edit?usp=sharing)
1. in kdenlive:
   1. add intro slide for same duration as intro jingle

TODO: set template so that duration of both match

   1. crop beginning and end of the video
   1. eventually do any other editing (for example: remove long pauses...)

1. render the video: `episode-[episode number]\_title_here.mp4`
1. extract the soundtrack of the video:
   `episode-[episode number]\_title_here.wav`
    1. open `.mp4` with audacity and `File --> Extract as .wav`
1. do simple noise removal on the soundtrack

   TODO  describe more for normal human beings

1. do sound leveling of the soundtrack with [Auphonic](https://auphonic.com/):
   `episode-[episode number]\_title_here.mp3`

   TODO describe more

1. replace old sound track with the new one
1. eventually add any extra "effects" (for example some fade to / out of black)
1. re-render the video
1. upload to youtube but do not publish yet
   1. update video_description
   1. add eventual extra video links on the outro slide
1. send link to speakers in the video to get their approval
1. publish on youtube
1. upload mp3 to anchor

## Issues

- templates will work only with absolute paths for the "clips" ?

- outro: GIF of a scroll of all contributors

## References

Podcast editing wiki:

- https://osf.io/exu5h/
- https://doi.org/10.1016/j.tics.2020.10.003
