# Radar_Target_Generation_Detection


<img src="https://user-images.githubusercontent.com/40875720/68837647-f8423a00-06f7-11ea-8abe-e9404b59e17f.PNG" width="600">
<img src="https://user-images.githubusercontent.com/40875720/68837656-fb3d2a80-06f7-11ea-9f80-229500210e15.PNG" width="600">
<img src="https://user-images.githubusercontent.com/40875720/68837659-fd06ee00-06f7-11ea-9adf-eedc78e20597.PNG" width="600">


## CFAR implementation

%design a loop such that it slides the CUT across range doppler map by
%giving margins at the edges for Training and Guard Cells.
%For every iteration sum the signal level within all the training
%cells. To sum convert the value from logarithmic to linear using db2pow
%function. Average the summed values for all of the training
%cells used. After averaging convert it back to logarithimic using pow2db.
%Further add the offset to it to determine the threshold. Next, compare the
%signal under CUT with this threshold. If the CUT level > threshold assign
%it a value of 1, else equate it to 0.


%Select the number of Training Cells in both the dimensions.
Tr = 8;
Td = 4;

%Select the number of Guard Cells in both dimensions
Gr = 4;
Gd = 2;

## Supree non thresholded edges
Do not need as I have initialeze the matrix with zeros

