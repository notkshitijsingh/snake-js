# Snake Game

A modern twist on the classic Snake game built using JavaScript, HTML, and CSS. The game features a dynamic grid system with increasing difficulty levels as the player progresses.

## Overview

This Snake game enhances the traditional gameplay with smooth animations, two difficulty modes (Easy and Hard), and fading effects that increase challenge over time. Players control the snake to eat apples while avoiding walls and self-collisions.

## File Structure

```
project-directory/
├── index.html       # Main HTML structure
├── script.js        # Game logic and animations
└── style.css        # Styling for game elements
```

### File Descriptions
- **index.html**: Contains the structure and initial layout, linking the CSS for styling and the JavaScript for game functionality.
- **script.js**: Implements the game mechanics, handling the snake’s movement, collisions, and scoring.
- **style.css**: Styles the grid, tiles, and controls the layout and responsiveness of the game screen.

## Game Elements

1. **Snake**: Moves across the grid, growing in length upon eating an apple.
2. **Apple**: Randomly appears on the grid for the snake to consume.
3. **Score**: Displays the current game score.
4. **Contrast**: The game’s visual contrast decreases over time, increasing difficulty.
5. **Difficulty Modes**:
   - **Easy Mode**: Regular game speed and fade rate.
   - **Hard Mode**: Increased speed and faster contrast fade.

## How It Works

1. **Start Game**: Press any arrow key or space bar to start moving the snake. Press 'H' to enable hard mode, and 'E' to switch back to easy mode.
2. **Movement**: Control the snake using the arrow keys.
3. **Gameplay Goal**: Eat as many apples as possible without colliding with the walls or the snake's body.
4. **Scoring**: Each apple consumed increases the score and resets the apple's position.
5. **Contrast Decay**: The game’s background fades progressively to make it harder to see the grid.

## Game Logic and Mathematics

1. **Grid System**: The game operates on a 15x15 grid. Each grid cell can be occupied by the snake or an apple.
2. **Snake Movement**: The snake moves continuously based on user input and cannot reverse direction. The head moves first, and each following segment moves to the position of the preceding one.
3. **Apple Placement**: Randomly placed on the grid, ensuring it does not overlap with the snake.
4. **Collision Detection**: The game checks for wall collisions (grid boundaries) and self-collisions. Hitting any boundary or the snake's body ends the game.
5. **Contrast Decay**: The contrast reduces based on the player’s score and the fade rate, making it challenging over time.

## Customization

- **Grid Size**: Modify the `width` and `height` in `script.js` to adjust the grid dimensions.
- **Snake Speed**: Change the `speed` variable in `script.js` to increase or decrease the snake’s movement speed.
- **Difficulty Settings**: Adjust the `fadeSpeed` and `fadeExponential` values for each mode to control the contrast decay rate and challenge level.
- **Color Scheme**: Modify colors in `style.css` to update the appearance.

## Running the Game

1. Clone the repository.
2. Open `index.html` in a web browser to start playing.

## Future Enhancements

1. **Sound Effects**: Add sound effects for actions like eating an apple or hitting a wall.
2. **High Scores**: Implement a high score tracker to record top scores across sessions.
3. **Level Progression**: Increase the grid size and speed as players reach higher scores.
4. **Mobile Compatibility**: Improve responsiveness and add touch controls for mobile users.
