# SoundCloud Audio Player Embedding

This guide explains how to embed a SoundCloud audio player in a web page, which plays audio automatically when the page loads. It also covers the parameters used to customize the player.

## How It Works

1. **HTML Structure**:
   - An `iframe` is used to embed the SoundCloud player.
   - The `#player` element is styled to ensure it fits well within the page.

2. **JavaScript Functionality**:
   - The script retrieves the SoundCloud track URL from the URL query parameters.
   - It constructs the embed URL using the provided track URL and specified parameters.
   - The constructed URL is assigned to the `src` attribute of the `iframe` to load and play the audio.

## Parameters

- **url**: The URL of the SoundCloud track. This is extracted from the query parameter `url-song` and should be a valid public SoundCloud track URL.
  
  Example:
https://soundcloud.com/the-business-34949400/shake-it-off-taylor-swift


- **auto_play=true**: Ensures that the audio starts playing automatically when the page loads.

- **hide_related=true**: Hides related tracks in the player.

- **show_comments=false**: Hides comments on the track.

- **show_user=false**: Hides the user profile who uploaded the track.

- **show_reposts=false**: Hides reposts of the track.

## Example Usage

To use this code, upload the HTML file to your web server and access it with the SoundCloud track URL as a query parameter. 

For example:

https://yourdomain.com/path/to/index.html?url-song=https://soundcloud.com/the-business-34949400/shake-it-off-taylor-swift


When accessed, the page will display the SoundCloud player embedded with the track specified in the URL and will start playing the audio automatically.

## Troubleshooting

- **404 Errors**: Ensure that the SoundCloud track URL is correct and publicly accessible.
- **Autoplay Issues**: Some browsers have restrictions on autoplay. Ensure that your browser settings allow autoplay for the page.

Feel free to modify the parameters or styles as needed to fit your requirements. If you encounter any issues or need further assistance, consult the [SoundCloud Developer Documentation](https://developers.soundcloud.com/docs/api/reference#resolve) for more details.
