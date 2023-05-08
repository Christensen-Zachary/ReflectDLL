# ReflectDLL

This project is to be used as a command line tool. 
This project creates a digraph of dependencies for classes found within the same DLL.
By giving the path to a DLL built using .NET, each classes dependencies are saved in a CSV file.
A python script is then used to parse the CSV file into a pdf of graph.

Example usage


  --Open terminal and change directory to the folder with the solution
  
  
  --Run the command "dotnet build"
  
  
  --Change directory to "./ReflectDLL/bin/Debug/net6.0" * the number after /net may vary *
  
  
  --Run the command "dotnet ./ReflectDLL.dll [pathToDLL]"
  
  
  --Move the generated CSV files "Dependencies.csv" and "TypeNames.csv" to the folder with the GraphDependencies.py file
  
  
  --Now, running ./GraphDependencies.py will output a digraph of the dependencies

Notes:

  Very large graphs may not be readable
  
  Results may include some erroneous types surrounded by angle brackets. These results are not graphed, but they are in the CSV
  
  
