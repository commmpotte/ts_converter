# Video Compression Utility (using ffmpeg)

This utility is designed to compress video files using ffmpeg. It allows users to input the width, height, file path, and output name of the compressed video. The application utilizes Node.js and the inquirer library for command-line prompts.

## Architecture Overview

### Core
- **Prompt**: Handles user input prompts using inquirer.
- **Files**: Manages file-related operations, such as file paths and file deletion.
- **Command Executor**: Abstract class responsible for executing commands.

### Commands
- **ffmpeg Builder**: Builds the ffmpeg command with specified parameters.
- **ffmpeg Executor**: Executes the ffmpeg command using child processes.

### Output
- **Console**: Displays output messages and status updates in the console.

## Features
- Modular architecture: The application is designed with modularity in mind, allowing for easy extension and modification of functionality without requiring a complete rewrite.
- Command Executor: The Command Executor abstract class provides a standardized interface for executing commands, allowing for easy addition of new commands in the future.
- Stream Processing: Video compression is performed using child processes, with output streams processed for logging and error handling.

## Installation and Usage
1. Clone the repository to your local machine.
2. Install dependencies by running `npm install`.
3. Run the application using `node dist/app.js`.
4. Follow the prompts to input the desired width, height, file path, and output name for the compressed video.
5. Once the process is complete, the compressed video will be available at the specified output path.

## Requirements
- Node.js
- npm
- ffmpeg (installed and added to system PATH)

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

## Some pics
<img width="872" alt="Снимок экрана 2024-02-16 в 12 20 07" src="https://github.com/commmpotte/ts_converter/assets/95095531/49f65610-7c5f-40f6-9c54-3c82b10dfa40">
<img width="872" alt="Снимок экрана 2024-02-16 в 12 20 21" src="https://github.com/commmpotte/ts_converter/assets/95095531/2e6e1dd4-cd6a-49fe-b654-a6d86f5414fa">
