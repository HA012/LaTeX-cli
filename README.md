# LaTeX-cli

Bash script that allows the user to (re)compile LaTeX files from the terminal and view the pdf output after each compilation process. 

## About the Script

The script is a wrapper around the tools included in [TeX Live](https://tug.org/texlive/). It is intended to be used in a separate terminal window, allowing the user to control the compilation process while editing the source file. After each compilation, the user is asked whether she wants to open the pdf output or recompile the file. If the pdf is already opened in another window, then opening the file will actually change focus to that window. The script also removes every auxiliary file generated during the compilation process - e.g., files whose extensions are aux, bbl, blg, log, nav etc.

By including the path to the script in PATH, the user will be able to run it from anywhere in the file system, and the output will be saved in the current working directory.

## Dependencies

	* texlive 
	* wmctrl
	* zathura 
	* zathura-pdf-mupdf 

## Instructions 

Assuming that FILENAME.tex is in the current working directory, and that the user has included the path to the script among the values of PATH (or moved the script to one of its previous values), run:        

>>$texc FILENAME.tex 

## Screenshots

![image_01](/images/image_01.png)

![image_02](/images/image_02.png)

![image_03](/images/image_03.png)

![image_04](/images/image_04.png)
