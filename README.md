# browser-
Search Browser using python 
## Code Readme

This code is a Python script that creates a simple graphical user interface (GUI) using the tkinter library. The GUI allows the user to enter a search query and opens the top 6 search results in their web browser.

### Prerequisites
To run this code, you need to have the following dependencies installed:
- youtube_dl
- urllib
- shutil
- webbrowser
- tkinter
- googlesearch

### Running the Code
To run the code, follow these steps:
1. Install the required dependencies if you haven't already.
2. Copy the code into a Python script file (e.g., `search_gui.py`).
3. Open a terminal or command prompt and navigate to the directory where the script is located.
4. Run the script by executing the command `python search_gui.py`.

### How it Works
1. The script starts by importing the necessary libraries and modules.
2. It creates a tkinter window by initializing an instance of the `Tk` class.
3. The window's size is set to 630x150 pixels, and the title is set to "Browser".
4. The background color of the window is set to '#fcfcec'.
5. A label is added to the window with the text "Enter what to search:", a background color of '#fcfcec', a foreground color of '#4b7fa4', and a font of size 20.
6. An entry field is added to the window with a width of 100 characters, a background color of "Black", a foreground color of "#cb464e", and a border size of 10.
7. A function named `pas` is defined. This function is called when the "Search" button is clicked.
8. Inside the `pas` function, the `search` function from the `googlesearch` module is used to perform a search query based on the text entered in the entry field.
9. The top 6 search results are retrieved, and each result is opened in the user's web browser using the `webbrowser.open` function.
10. A button named "Search" is added to the window with a background color of '#cb464e', a foreground color of '#fcfcec', and a font of size 20. When clicked, this button calls the `pas` function.
11. The label, entry field, and button are arranged in a grid layout using the `grid` method.
12. Finally, the `mainloop` method is called to start the tkinter event loop and keep the window open until it is closed.

### Modification and Extension
- You can customize the size and appearance of the window by modifying the `geometry`, `title`, and `configure` functions.
- You can change the text and appearance of the label and button by modifying the respective `Label` and `Button` instances.
- You can add additional functionality to the code, such as saving the search results to a file or displaying more information about each search result.

### Limitations
- The code currently only supports searching with the 'co.in' top-level domain. You can modify the `tld` parameter in the `search` function to use a different top-level domain.
- The code only opens the search results in the default web browser. If you want to open the results in a specific browser, you can modify the `webbrowser.open` function to specify the browser executable path.
- The code does not handle errors or exceptions that may occur during the search or web browser opening process. Adding error handling and exception catching can make the code more robust.
