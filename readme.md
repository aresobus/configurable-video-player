# NBC Universal Configurable Video Player

 This video player is designed specifically for various brands under the NBC Universal group, providing a highly customizable interface that supports both VOD and live streaming services.

## Features

- **Configurable Playlist**: Supports a dynamic playlist configurable per brand requirements.
- **Responsive Design**: Adapts to different screen sizes and orientations.
- **Live and VOD Streaming**: Capable of handling both live and video-on-demand streaming.
- **Customizable UI**: Allows brands to apply their theming and control elements visibility.

## Configuration

The player can be configured with a JSON object that specifies various options such as the playlist, UI behaviors, theming, and more. Below is an example configuration with sample values:

```json
{
    "playlist": [
        {
            "videoSrc": "assets/img/sing.mp4",
            "coverImgSrc": "assets/img/sing-movie-animals.jpg",
            "title": "The Sing Movie",
            "subtitle": "In Theaters August 19",
            "description": "A group of animals that enter a singing competition, hosted by a koala hoping to save his theater."
        },
        {
            "videoSrc": "assets/img/secret-life-of-pets-trailer3.mp4",
            "coverImgSrc": "assets/img/secret-life-of-pets-poster.jpg",
            "title": "Pets the movie Trailer",
            "subtitle": "In Theaters July 8",
            "description": "The quiet life of a terrier named Max is upended when his owner takes in Duke, a stray whom Max instantly dislikes."
        }
    ],
    "initialPlaylistIndex": 0,
    "aspectRatio": 1.8497109826589595,
    "endCardShowTime": 0,
    "playNextDelay": 14,
    "enableSquezeCardControls": false,
    "controlBarHoverTimeout": 2,
    "hasSkipButton": false,
    "playerMode": "vp-mode-vod",
    "endCardLinks": [
        {
            "text": "Some link 1",
            "url": "http://blah.com"
        },
        {
            "text": "Some link 2",
            "url": "http://blah.com"
        }
    ],
    "adRoll": false,
    "sharePlatforms": [
        "facebook",
        "twitter",
        "googleplus"
    ],
    "allowEmbed": true,
    "allowShare": true,
    "theme": {
        "colorHighlight": "#33b5d5"
    }
}
```

## Installation

To get the video player running locally:

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Start the Development Server**:
   ```bash
   gulp
   ```
   This will load the player in a browser on `localhost:3000`.

### Requirements

- Node.js 6.0+ is recommended for optimal compatibility.

### Sites

- **Raw Player**: Accessible at `http://localhost:3000`
- **Crisp Video Generator**: Located at `http://localhost:3000/crisp.html`

## Live Prototype

A live prototype of the video player can be viewed [here](https://rationalized-player.nbcuxlab.com/crisp.html).

## License

This project is licensed under the MIT License. Created by Alex Lebedyev (oleksandr.lebedyev@nbcuni.com)