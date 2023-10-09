# React / NextJS Audio Player

## Introduction

This is a simple yet powerful audio player built using Next.js and TailwindCSS. It's designed to provide a seamless audio playback experience with a clean and intuitive UI. The audio player is also compatible with React, making it versatile and easy to integrate into various web projects.

## Features

#### Basic Playback Controls
- **Play/Pause**: Control the playback of the current song.
- **Next/Previous**: Skip to the next or previous song in the playlist.
- **Progress Bar**: Navigate through the current song with ease.

#### Song List
- **Selectable Songs**: Click on a song in the list to play it.
- **Song Duration**: Displays the duration of each song next to its title.
- **Current Song Title**: Shows the title of the current song being played.

#### Time Formatting
- **Current Time**: Displays the current time of the song in minutes and seconds.

#### Auto Play Next
- **Looping**: Automatically plays the next song in the list when the current one ends.

## Installation and Usage

### Creating a New Project Based on the Audio Player

1. **Clone the Repository**
    ```bash
    git clone https://github.com/tobiasvdorp/nextjs-audio-player.git
    ```
2. **Install Dependencies**
    ```bash
    npm install
    ```
3. **Start Development Server**
    ```bash
    npm run dev
    ```

### Integrating the Audio Player into an Existing Project

1. **Copy Components**
    - [`AudioPlayer.js`](https://github.com/tobiasvdorp/nextjs-audio-player/blob/main/nextjs-audio-player/src/components/AudioPlayer.js)
    - [`BottomUI.js`](https://github.com/tobiasvdorp/nextjs-audio-player/blob/main/nextjs-audio-player/src/components/BottomUI.js)
    - [`Song.js`](https://github.com/tobiasvdorp/nextjs-audio-player/blob/main/nextjs-audio-player/src/components/Song.js)

2. **Install Dependencies**
    ```bash
    npm install react-icons
    ```

3. **Import Components**
    ```javascript
    import AudioPlayer from './path/to/AudioPlayer';
    ```

4. **Add the Audio Player**
    ```javascript
    <AudioPlayer />
    ```

5. **Add Songs**
    ```javascript
    // Example list of songs
    const songs = useMemo(
      () => [
        {
          id: "1",
          title: "Flute",
          src: "/flute.wav",
        },
        // Add more songs here
      ],
      []
    );
    ```

6. **Customize the UI**
    - Modify `BottomUI.js` and `Song.js` to customize the UI.
    - Customize the color palette by modifying the colors in `tailwind.config.js`.

## Dependencies

- React / NextJS
- React Icons
- TailwindCSS

## Contributing

Feel free to open issues or submit pull requests to contribute to the improvement of this audio player.

## Conclusion

You should now have successfully integrated the React / Next.js Audio Player into your existing project. Feel free to customize it further to fit your needs.
