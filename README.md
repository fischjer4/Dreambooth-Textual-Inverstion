As of 10/1/22 this must be run on a GPU with at least 24gb vRAM and 60gb volume memory.
I use RunPod.io RTX5000

Initial Setup:

1. Get about 20 images of a person - front, side, back, face, body
2. Crop the images so it’s just the person
3. Convert all images to 512x512 using something like [https://www.birme.net](https://www.birme.net/)
4. Go to RunPod and select a GPU that has at least 24gb of vRAM
5. When setting up the GPU, change the Container Disk and Volume Disk to 60
6. For the Template dropdown, select RunPod Stable Diffusion and make sure the Start Jupyter Notebook is checked
7. Deploy On Demand (otherwise others can interrupt it)
8. Go to MyPods > drop down toggle for your pod > Connect > Connect to Jupyter lab
9. In the Jupyter Notebook select Python 3 to open a new window
10. Enter `!git clone https://github.com/fischjer4/Dreambooth-Textual-Inverstion.git`
    - This will clone the DreamBooth Textual Inversion repo inside of your Jupyter workspace folder
11. You can discard the window used to clone now
12. Open the repo folder and double click on the orange file named `train_your_images`
    - This is going to prepopulate a new window with all of Jupyter cells filled in that is needed to run this
