**************************************************************************************
McCadDecomposer: A SpaceClaim linked tool for decomposing CAD to Constructive Solid Geometry (CSG). 

McCadDecomposer is a sub-function of McCad program. It can be linked from the SpaceClaim CAD software to make interactive decomposition on the CAD geometry, to prepare for the conversion to Monte Carlo (MC) CSG geometry.

**************************************************************************************

This package contains three main items

  * McCadDecomposer: the folder containing the McCadDecomposer.exe and another libraries. 
  * McCadDecomposer_SpaceClaim_v0.1.scscript: a SpaceClaim python script which links the McCadDecomposer with SpaceClaim
  * Examples: some example solids.
  * README.md: this file

********Installation and useage********  
To use this package, you need SpaceClaim version 2016 (R 17.1) or later.

* Download the package in to a folder, here brief as $MCCAD. 
   * Please noted that the folder name of any upper level folder should NOT start with character "t" and "n" due to python linguistics. 
   
   * For example, folder "D:\tomorrow\now" is a bad folder to place this package. 

* Start SpaceClaim, and load the example CAD model which needs to be decomposed.

* Load the conversion script. 
   * click File->Open, change folder to $MCCAD 
   
   * select the file type "SpaceClaim Script (*.scscript, *.py)" at the right-below corner    
   
   * select the McCadDecomposer script "McCadDecomposer_SpaceClaim_v0.1.scscript". 
   * the script will be display along side with the CAD model.

* Using the script to decompose CAD model.
   * For the fisrt time, you have to provide the path of the McCadDecomposer.exe to the script. In the very begin of the script "User Input" provide the full path of "$MCCAD\McCadDecomposer" to the variable "PathToMcCad". 
   
   * Selete one or more solids, and click the green Play button to run the script. Noted that no selection or selecting the component does not work.

********General Suggestion********    

* When McCadDecomposer is failed, try to help it with manual cut on the CAD model and make it less complex for decomposition.

* Check the ouptut message in order to find the error, e.g. Spline surface. 

********!!! SpaceClaim Crash !!!********  
* Sometimes SpaceClaim graphic will crash due to too fast graphical refreshing. If you encounter this problem, here is some way to mitigate the problem:
   
   * At File->SpaceClaim Options->Advanced, UNCHECK the option "Animate Changes to the view projection".
   
   * Minimize the SpaceClaim window during the script running. 
   

for further information or question please contact yuefeng.qiu@kit.edu. 
   
