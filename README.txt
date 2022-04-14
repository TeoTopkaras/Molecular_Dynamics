Code simply runs without any input from an external file, exept for the calculation of the pair correlation function. In order to simulate different 
states, you have to change the State_set parameter in the main simulation block. The code does approximately 20 minutes to run.

For the preseted parameters we have the following settings:

------------------------------------------------
State_set = 1, Gas state simulation 

State_set = 2, Liquid state simulation 

State_set = 3, Solid state simulation 
------------------------------------------------

In addition, for the pair correlation function you have to set the cor_func_factor in order to plot the correct g.

------------------------------------------------
cor_func_factor = 1, Gas state simulation 

cor_func_factor = 2, Liquid state simulation 

cor_func_factor = 3, Solid state simulation 
------------------------------------------------



In case you want to see how the simulation progress in a video, you have to run the imported libraries 
twice.

The only not optimized function of the code is the pair correlation function. The way it works now is, 
you have to run the simulation as many times as you want, and each time you have to save the file with 
a different name. After that, you can take the mean of that and plot the pair correlation function for the 
corresponding state of matter. For reference, for our plots we have made five simulations for each state.