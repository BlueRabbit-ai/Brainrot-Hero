## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Project Structure](#project-structure)
- [Changing the Displayed Text](#changing-the-displayed-text)
- [Customizing Colors](#customizing-colors)
- [Adjusting Game Parameters](#adjusting-game-parameters)
- [Deployment](#deployment)
- [Troubleshooting](#troubleshooting)

## Introduction
BlueRabbit is a modern, interactive web-based game that combines the classic Pong mechanics with innovative pixel text display. It's built using React and Next.js, offering a unique and engaging user experience.

## Features
- Responsive design that adapts to various screen sizes
- Dynamic pixel text display for game title and subtitle
- Pong-like gameplay with four paddles and a bouncing ball
- Color-changing elements for enhanced visual appeal
- Customizable text and color schemes

## Installation
To install and run BlueRabbit locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/BlueRabbit-ai/Brainrot-Hero.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Brainrot-Hero
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Run the development server:
   ```bash
   npm run dev
   ```
5. Open your browser and visit `http://localhost:3000`

## Usage
Once the game is running, you'll see the pixel text display of the title and subtitle. The ball will start moving automatically, and the paddles will try to intercept it. The game continues indefinitely, with the ball changing color upon hitting edges or paddles.

## Configuration
You can customize various aspects of the game by modifying the `config.ts` file located in the `app` directory. Here's how to change the displayed text:

1. Open `app/config.ts`
2. Locate the `CONFIG` object
3. Modify the `TITLE` and `SUBTITLE` properties:
   ```typescript
   export const CONFIG = {
     TITLE: "Your New Title",
     SUBTITLE: "Your New Subtitle",
     // ... other configuration options
   }
   ```
4. Save the file and the changes will be reflected immediately in the development server

You can also adjust colors, speeds, and other game parameters in this file.

## Contributing
Contributions to BlueRabbit are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch: `git checkout -b feature-name`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
If you have any questions, issues, or suggestions, please open an issue on the GitHub repository or contact the maintainer at [your-email@example.com](mailto:your-email@example.com).

Enjoy playing and modifying BlueRabbit!

## Project Structure
The BlueRabbit project is structured as follows:

```
/bluerabbit
  /app
    /components
      BlueRabbit.tsx
    config.ts
    page.tsx
  README.md
  package.json
  tsconfig.json
  next.config.js
```

### Key Files:
1. `app/components/BlueRabbit.tsx`: This is the main game component. It handles the game logic, rendering, and interactions.
2. `app/config.ts`: Contains the configuration for the game, including text, colors, and game parameters.
3. `app/page.tsx`: The main page component that renders the BlueRabbit game.
4. `package.json`: Lists the project dependencies and scripts.
5. `tsconfig.json`: TypeScript configuration file.
6. `next.config.js`: Next.js configuration file.

## Changing the Displayed Text
To change the text displayed in the game:

1. Open `app/config.ts`
2. Find the `CONFIG` object
3. Update the `TITLE` and `SUBTITLE` properties:
   ```typescript
   export const CONFIG = {
     TITLE: "Your New Title",
     SUBTITLE: "Your New Subtitle",
     // ... other properties
   }
   ```
4. Save the file
5. If the development server is running, the changes will be reflected immediately

## Customizing Colors
You can also customize the game's color scheme in the same `config.ts` file:

1. Open `app/config.ts`
2. Locate the `COLOR_PALETTE` array in the `CONFIG` object
3. Modify the colors as desired. For example:
   ```typescript
   COLOR_PALETTE: [
     "#4B0082", // Indigo (key color)
     "#6A5ACD", // Slate Blue
     "#8A2BE2", // Blue Violet
     "#9370DB", // Medium Purple
     "#7B68EE", // Medium Slate Blue
     "#BA55D3", // Medium Orchid
   ],
   ```
4. You can also change individual element colors:
   ```typescript
   BACKGROUND_COLOR: "#000000",
   TEXT_COLOR: "#FFFFFF",
   HIT_COLOR: "#9370DB",
   BALL_COLOR: "#BA55D3",
   PADDLE_COLOR: "#6A5ACD",
   ```
5. Save the file to see the changes

## Adjusting Game Parameters
To modify game behavior:

1. Open `app/components/BlueRabbit.tsx`
2. Find the `initializeGame` function
3. Adjust values like `BALL_SPEED`, paddle sizes, or game scaling factors

Remember to test thoroughly after making changes to ensure the game still functions correctly across different screen sizes.

## Deployment
To deploy BlueRabbit:

1. Build the project:
   ```bash
   npm run build
   ```
2. Start the production server:
   ```bash
   npm start
   ```
3. Or, deploy to a platform like Vercel:
   - Push your code to a GitHub repository
   - Connect the repository to Vercel
   - Vercel will automatically deploy your application

## Troubleshooting
If you encounter issues:

1. Ensure all dependencies are installed: `npm install`
2. Clear the Next.js cache: `rm -rf .next`
3. Restart the development server
4. Check the console for error messages
5. Verify that your Node.js version is compatible with the project

For more help, consult the Next.js documentation or open an issue on the GitHub repository.

Enjoy BlueRabbit! 