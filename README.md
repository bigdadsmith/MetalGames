# MetalGames

macOS application for managing and running Windows games using Wine and GPTK.

## About the Project

MetalGames is a macOS application being developed as a launcher to simplify running and managing Windows games and applications within the Wine or Game Porting Toolkit environment. The project is under active development and is a personal project.

## Features

Currently, the application is capable of:

* Adding programs/games to the list by selecting their `.exe` or `.app` file.
* Creating and managing separate Wine/GPTK "bottles" (prefixes) for each added program to prevent conflicts.
* Launching the Wine process with the selected program.
* Stopping the running Wine process.
* Displaying the standard output (stdout) and standard error output (stderr) of the Wine process for debugging.
* Saving and automatically loading the list of added programs on application launch (persistence).
* Allowing manual specification of the Windows path to the executable inside the bottle for more correct launching of installed programs.

## Getting Started (for Developers)

To build and run the project from source:

1.  Ensure you have Xcode and the necessary command-line tools installed.
2.  Ensure you have Wine or Game Porting Toolkit installed (e.g., via Homebrew).
3.  Clone this repository.
4.  Open the project file (`.xcodeproj` or `.xcworkspace`) in Xcode.
5.  In your project settings in Xcode, under the "Signing & Capabilities" tab, temporarily **disable App Sandbox** to allow the application to launch external processes (`Process`) and access files outside its sandbox during development.
6.  In the `GameDetailView.swift` file (where the `launchGame` function is), ensure the path to the Wine binary (`let wineBinaryPath = ...`) is specified correctly for your system.
7.  Build and run the application in Xcode.

## Requirements

* macOS Operating System 14+
* Apple Silicon (Mac M1-M4)
* Xcode 16
* An installed Wine or Game Porting Toolkit binary
