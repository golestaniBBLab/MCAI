<pre>

 _____ ______   ________  ________  ___     
|\   _ \  _   \|\   ____\|\   __  \|\  \    
\ \  \\\__\ \  \ \  \___|\ \  \|\  \ \  \   
 \ \  \\|__| \  \ \  \    \ \   __  \ \  \  
  \ \  \    \ \  \ \  \____\ \  \ \  \ \  \ 
   \ \__\    \ \__\ \_______\ \__\ \__\ \__\
    \|__|     \|__|\|_______|\|__|\|__|\|__|
                                            

</pre>
by Josue Luiz Dalboni da Rocha

## Paper

Multivariate Concavity Amplitude Index (MCAI) for characterizing Heschl’s gyrus shape.Josue Luiz Dalboni da Rocha, Olga Kepinska, Peter Schneider, Jan Benner, Letitia Schneider, Narly Golestani.

## Usage Manual

# Installation

This software has been written in Matlab. Download the folder containing the code and add it to you Matlab path with 
```matlab
addpath(PathtoFolder/MCAI)
```

# Processing the data
This toolbox operates as an extension of TASH. Heschl’s gyrus masks obtained from the toolbox are thus mandatory. Follow the User Manual of TASH to get them! 
The following Concavity Indexes are extracted using MCAI:

*MCAI_[lh,rh]_total MCAI values independent of orientation 
*MCAI_[lh,rh]_[orientationType] MCAI results for one specific orientation. Lateral, Medial, Anterior, et. (see comment MCAI for a full description)

To use the toolbox navigate to the folder where you want to extract the MCAI images and simply run:
```matlab
MCAI=MCAI(D_load)
```
Where D_load is the folder containing the .tif output of TASH toolbox for the left AND right hemispheres.
The MCAI structure will contain matrices NxM where N is the number of subjects and M the 4 dominant concavity indices in the direction of interest (or independent of orientation)
