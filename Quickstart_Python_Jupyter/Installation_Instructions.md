# Getting Started with Anaconda for Linux/Mac and Windows

## Installing Anaconda

### For Linux/Mac

1. **Download Anaconda:**
   Go to the [Anaconda Distribution page](https://www.anaconda.com/products/distribution) and download the Python 3 installer script for your system.
   ```
   wget https://repo.anaconda.com/archive/Anaconda3-latest-Linux-x86_64.sh
   ```
2. **Change the mode of the downloaded script to executable:**
   ```
   chmod +x Anaconda3-latest-Linux-x86_64.sh
   ```
3. **Run the installation process:**
   ```
   ./Anaconda3-latest-Linux-x86_64.sh
   ```
4. **Follow the on-screen instructions:**
   At the end, the script will offer to add the Anaconda installation location to the PATH in your .bashrc/.bash_profile. You should say 'yes'.
   ```
   # added by Anaconda3 installer
   export PATH="/Users/yourusername/anaconda3/bin:$PATH"
   ```
5. **Open a new terminal window and type:**
   ```
   conda
   ```
   If you see the conda help, then everything is set up properly.
   
### Windows
1. **Download Anaconda:**
   Go to the [Anaconda Distribution page](https://www.anaconda.com/products/distribution) and download the Python 3 installer script for Windows.
2. **Run the installer and follow the on-screen instructions.**
   If the installation is successful, you will have Anaconda installed.
3. **Open the Anaconda Prompt from the Start menu and type:**
   ```
   conda
   ```
   If you see the conda help, then everything is set up properly.

## Setting Up the Environment
1. **Add the conda-forge channel:**
   ```
   conda config --add channels conda-forge
   ```
2. **Create the environment using the `environment.yml` file:**
   Download the `environment.yml` file provided to you for the course. Navigate to the directory where the `environment.yml` file is located and run:
   ```
   conda env create -f environment.yml
   ```
3. **Activate the environment:**
   ```
   conda activate your_environment_name
   ```

## Launching Jupyter Notebook
1. **Start Jupyter Notebook:**
   ```
   jupyter notebook
   ```
2. **The browser should open with the Jupyter main page.**
   You can navigate to the folder with your notebooks from there and open them.


By following these instructions, you should have everything set up properly to begin working with Python and Jupyter Notebooks.
