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

## Requirements

* macOS Operating System 14+
* Apple Silicon (Mac M1-M4)
* Xcode 16
* An installed Wine or Game Porting Toolkit binary
