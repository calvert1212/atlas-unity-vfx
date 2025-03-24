# WAYSEND\ \PARIAH
![WaysendScreenshot](https://github.com/user-attachments/assets/30b46abc-97a1-4a2a-96aa-c795e342fb22)

## Overview
WaysendPariah is a Unity-based 2D Asteroids-like space shooter combined with beat detection-enhanced gameplay camera control functionality for navigation in a 2D or 3D environment.

## Features
- Keyboard-controlled camera movement
- Adjustable camera movement speed
- Smooth integration with Unity's input system

## Getting Started

### Prerequisites
- Windows 10 or newer OR MacOS
- Unity 2019.4 or newer (recommended)
- Basic understanding of Unity's coordinate system

### Installation
1. Clone the repository:
```bash
git clone https://github.com/calvert1212/WaysendPariah.git
```

2. Open the project in Unity:
   - Launch Unity Hub
   - Click "Add" and browse to the cloned repository
   - Select the project folder and open it

## Usage

### Camera Movement System
The camera automaticcally follows the player's ship's position.

#### Key Functions:
- `BeatDetector.cs`
Detects the beat of the music and modifies gameplay elements accordingly.
Adjusts beat detection settings based on genre.

- 'Jukebox.cs' and 'Playlist.cs
Plays the music and handles the beat detection.

#### How to Use:
1. After cloning the repository, open the project in Unity. If you want to make any changes, you may do so in the editor now.
2. Change the Build platform to either Windows or MacOS.
3. Build the game and run it on your desired platform.

```csharp
// Example of how the camera movement works
float moveX = Input.GetAxis("Horizontal"); // Left/Right arrow keys or A/D
float moveY = Input.GetAxis("Vertical");   // Up/Down arrow keys or W/S
Vector3 movement = new Vector3(moveX, moveY, 0) * moveSpeed * Time.deltaTime;
transform.position += movement;
```

## Customization
You can customize the playlist by adding or removing songs from the `Playlist` array in the `BeatDetector` script.
1. Open the `BeatDetector` script.
2. Modify the `Playlist` array to include or remove songs.
3. Save the changes and rebuild the game.


- **Move Speed**: Controls how quickly the camera moves in response to key presses
  - Increase for faster movement
  - Decrease for more precise control

## Troubleshooting

### Common Issues

### Excess velocity
-I haven't figured out a good way to reduce the ship's velocity without making the gameplay jarring and frustrating. Try to manage your speed so you don't end up in an extremely high-speed collision, make good use of your port/starboard thrusters (Q and E keys)!

#### Camera Moves Too Fast/Slow
- Adjust the `moveSpeed` parameter in the Inspector for the `CameraMoveWithKeys` component

#### Camera Not Responding to Input
- Ensure the script is attached to the active camera
- Verify that Unity's Input Manager has the correct key bindings for "Horizontal" and "Vertical" axes
- Check the Console for any error messages

## Contributing
Contributions to WaysendPariah are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Unity Technologies for the amazing game engine
- All contributors who have helped shape this project
- FEATURED MUSICAL ARTISTS:
  - Kingslayer by Bring Me the Horizon ft. BABYMETAL. Sony Music Entertainment UK
    - https://www.youtube.com/watch?v=fKyXvNkGQKc
  - CRAZY FUCKIN ROBOT BODY by SnowBlood, Mystery Skulls, and Gosteffects.
    - https://www.youtube.com/watch?v=t3qIbFeOAWM
  - Cascada - Everytime We Touch (Fallen Superhero Hardstyle Remix)
    - https://www.youtube.com/watch?v=5u37UGiSiL8
  - Our Truth by Lacuna Coil. Century Media 2006.
    - https://www.youtube.com/watch?v=SB9LXpO6yWo

##Authors
- Chad Calvert (https://github.com/calvert1212)
---
