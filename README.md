# Plyr Video Playlist

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

[Demo](https://plyr-video-playlist.dml0b3i.repl.co)

[![Screenshot of Playlist](https://github.com/vitordml/plyr-video-playlist/blob/main/plyr-video-playlist-scrnsht.jpg)](https://plyr-video-playlist.dml0b3i.repl.co)


## Description

This project is a web application that provides a user-friendly interface for a Playlist for the Plyr Media Player.

## Features

- Handles Youtube, Vimeo, HTML5/MP4 Video files. 
- Responsive design with a two-column layout
- Collapsable playlist button
- Watched item tracking in the playlist
- Video player with playlist integration
- Hides all vimeo/youtube embed controls/ recommended videos
- Search functionality
- Filtering by category functionality

## Dependencies

This project utilizes the following dependencies:

- [Plyr](https://github.com/sampotts/plyr): A simple, accessible, and customizable HTML5 media player.
- [Simplebar](https://github.com/Grsmto/simplebar): A custom scrollbar plugin that aims to be as easy to use as possible while maintaining performance and extensibility.

## Getting Started

To get a local copy up and running, follow these simple steps:

### Prerequisites

- A web browser

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/vitordml/plyr-video-playlist/.git
   ```
2. Open the project folder.
3. Open the `index.html` file in your preferred web browser.

## Usage
This playlist requires Playlist Items to be added in the following format:
```
<div class="playlist_item" data-title="" data-author="" data-purl="" data-video="" data-type="" data-category="">
   <div class="item_wrapper">
     <div class="item_thumb_container">
       <img class="item_thumb"
         src="">
       <div class="item_thumb_play"></div>
       <div class="item_thumb_restart"></div>
     </div>
     <div class="item_details">
       <span class="item_title"></span>
       <span class="item_director"></span>
     </div>
   </div>
</div>
```

- **data-title** / **data-author** atttributes are used to display the items information in the top left.
- **data-purl** handles any thumbnail image
- **data-video** handles the Youtube link, Vimeo ID or the html/mp4 video link
- **data-type** specified the media type, this is either youtube| vimeo | video
- **data-category** will be used to populate the **All** dropdown accordian menu in order to filter the playlist item. 

The remaining dom elements are **NOT** automatically filled in based on the data-attributes on load and need to be added manually for now. 
The playlist autoplays, and displays a buffering animation while the Plyr *progress* event is occuring.


## Contributing

Contributions are welcome! If you have any ideas, enhancements, or bug fixes, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Credit
I used the playlist code by [Skerbis](https://codepen.io/skibbi/pen/NWvLoRz) as a starting point


