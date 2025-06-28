# Pygame Self-Driving Car Demo

This minimal Pygame application demonstrates basic “autonomous” car navigation on a pre-rendered track.  
A Tesla sprite moves along the road by sampling pixel values in front of the vehicle and adjusting its direction when the colour pattern changes.

## Key Points
- **Computer vision by pixel sampling** – The script reads pixels at a fixed focal distance to detect white road areas (RGB 255, 255, 255).
- **Four-direction logic** – The car rotates and updates offsets to follow turns in the track.
- **Frame-rate control** – `pygame.time.Clock()` limits execution to 60 FPS.

## Requirements
- Python 3.8+  
- `pygame` 2.x  
- `track6.png` (track background)  
- `tesla.png` (car sprite)

Install Pygame:

```bash
pip install pygame
