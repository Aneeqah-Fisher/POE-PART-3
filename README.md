# POE-PART-3
CYBERSECURITY
# Cybersecurity Awareness Bot

## Overview
This project is a cybersecurity awareness chatbot implemented in C#. It includes both a console-based version and a WPF (GUI) version. The bot helps users learn about cybersecurity topics such as password safety, phishing, scams, and online privacy through interactive chat and predefined questions. It also incorporates audio greetings using the NAudio library.

---

## Features
- **Console Version:**
  - Text-based interaction with user input
  - Plays greeting audio file
  - ASCII art display
  - Personalized user interaction
  - Multiple predefined responses and topics
  - Supports both free text questions and numbered options
  
- **WPF Version:**
  - Graphical user interface with chat window
  - Buttons for quick questions
  - Plays greeting and responses sounds
  - Dynamic chat display
  - Easy to extend with more features

---

## Requirements
- Windows OS
- Visual Studio 2022 or later
- .NET Core 3.1, .NET 5, .NET 6, or newer
- NuGet package: **NAudio** (for audio playback)

---

## Setup Instructions

### For Console Version
1. **Clone or Download the Repository**
2. Open the solution in Visual Studio.
3. Ensure the `NAudio` package is installed:
   - Right-click on the project > Manage NuGet Packages
   - Search for `NAudio` and install the latest version
4. **Configure the audio file path**
   - Place your `Greeting.wav` in a known directory
   - Update the path in the `PlayGreeting()` method:
     ```csharp
     string musicDirectoryPath = @"C:\path\to\your\audio\folder";
     ```
5. **Build and Run**
   - Press F5 to start the console app
   - Interact with the chatbot via text input

### For WPF Version
1. **Create or open the WPF project**
   - Create a new WPF App (.NET Core/.NET 5/6/7)
2. **Install NAudio**
   - Manage NuGet packages, install `NAudio`
3. **Set up the UI**
   - Replace `MainWindow.xaml` with your design (see example below)
4. **Add your `Greeting.wav`**
   - Place it in an accessible location
   - Update the file path in `MainWindow.xaml.cs` in the `PlayGreeting()` method
5. **Build and run**
   - Press F5 to launch the GUI
   - Interact through chat and buttons

---

## Usage
- **Console Mode:**
  - Enter your name and favorite color
  - See ASCII art and get a personalized greeting
  - Ask questions or select numbered options
  - Type "exit" to quit

- **WPF Mode:**
  - Launch the app
  - Hear greeting sound
  - Use chat input or predefined buttons to interact
  - View responses in chat window

---

## Extending the Bot
- Add more predefined questions/buttons in WPF or console
- Improve response logic and topics
- Add more sounds or images
- Persist user data or preferences

---

## Troubleshooting
- **Sound not playing?**  
  Verify the WAV file path and existence. Check your audio device settings.

- **Build errors?**  
  Ensure `NAudio` NuGet package is installed and references are correct.

- **Runtime errors?**  
  Check for correct file paths, permission issues, and dependencies.

---

## License
This project is for educational and demonstration purposes. Feel free to modify and extend.

---

## Contact
For questions or feedback, contact [Your Name] at [your.email@example.com].

---

**Note:** Replace placeholder texts like `[Your Name]` and `[your.email@example.com]` with your actual info.
