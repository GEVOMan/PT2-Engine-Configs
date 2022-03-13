# PT2-Engine-Configs
Engine config files for RLCPT2 use with my soundsets.
All of these should be drop-in configs to be put in your ptgamma/engines directory in expression2, except for the EMD 16-710G3C-T2 and the GE 7FDL16Y9. For the EMD 16-710G3C-T2 and the GE 7FDL16Y9, you must make an edit to RLCPT2 for them to work to their best potential. See below.
# PT2 Edit (if necessary)
At line 456, you will find a statement that looks like this:

![image](https://user-images.githubusercontent.com/69711669/158041204-631f8fbd-38f7-4452-af56-bccec6759598.png)

## For the sounds to work properly, you must remove the equation that divides the soundDuration by variable SoundMultiplier like such:

![image](https://user-images.githubusercontent.com/69711669/158041224-4b19783a-2daa-4c43-a430-1ba55faa962c.png)

## I recommend making a variable that allows this process to be toggled on and off. Here is an example of such:

##Add variable in config of E2

![image](https://user-images.githubusercontent.com/69711669/158041234-b8fbd7d9-4a34-4416-9204-453e78567082.png)

#### Persist variable at the top of the E2

![image](https://user-images.githubusercontent.com/69711669/158041265-b1c1fc25-25ee-41f8-a6ef-80480494cafa.png)

#### Insert "if" statement where variable DR was defined (near line 453 as stated earlier)

![image](https://user-images.githubusercontent.com/69711669/158041188-d4633ba8-fbce-448c-a577-7abefd6d0385.png)



