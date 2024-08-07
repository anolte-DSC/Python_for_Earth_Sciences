# Getting Started with Anaconda for Windows and Linux/Mac

## Installing Anaconda
   
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

## Setting Up the Environment
1. **Add the conda-forge channel:**
   ```
   conda config --add channels conda-forge
   ```
2. **Create or update the environment using the `environment.yml` file:**

   2.1 **Create:**
   Creating isolated environments helps maintain clean and manageable development workflows, preventing package conflicts and ensuring reproducibility of your projects.
   Use the `environment.yml` file from the respective course section. Navigate to the directory where the `environment.yml` file is located and run:
   ```
   conda env create -f environment.yml -n your_environment_name
   ```
   You can also add the file location in the path to the `environment.yml`, for example:
   ```
   conda env create -f C:/Users/Username/Documents/A_Quickstart_Python_Jupyter/environment.yml -n your_environment_name
   ```
   
   2.1 **Update:**
   You can also update the packages in an existing environment using the `environment.yml` file from the respective course section. Make sure your target environment is activated for this to work.
   ```
   conda env update --file environment.yml
   ```
   You can also add the file location in the path to the `environment.yml`, for example:
   ```
   conda env update --file C:/Users/Username/Documents/A_Quickstart_Python_Jupyter/environment.yml
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
