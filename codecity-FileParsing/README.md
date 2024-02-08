Code city - file parsing by Thomas Choboter
This story centers around collecting information from java files and making that information accessible to the rest of the program.

JavaParser is created with a constructor that takes in a String path argument. This argument can point to a file or a directory.
If the path is a file, JavaParser makes a list of FileInfo objects with a size of 1. FileInfo objects have attributes for
the number of fields in the class, number of methods in the class, the class's name and the package name.
If the path is a directory, the list of FileInfo objects contains every java file contained within that directory.


In Main.java, a FileParser is created and set to search through the dummy_classes folder, which contains 5 java files within it.
It then calls toString for each FileInfo object present in the FileParser's list. The expected printout is this:

Class name: Bench  
Package name: parks
# Methods: 2       
# Attributes: 5
Class name: Bird
Package name: parks
# Methods: 9
# Attributes: 5
Class name: Car
Package name: vehicles
# Methods: 5
# Attributes: 5
Class name: Duck
Package name: parks
# Methods: 11
# Attributes: 7
Class name: Spaceship
Package name: vehicles
# Methods: 3
# Attributes: 6