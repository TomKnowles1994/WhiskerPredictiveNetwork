# WhiskerPredictiveNetwork
Code accompanying the Robotics MSc Project "Predictive coding applied to the removal of tactile reafferent noise"

## To Review

- Simply click on the Whisker Predictive Network v1 and/or v2 files in the repository. As they are Jupyter Notebooks, most of the outputs have been stored with the code.

- v1 is the network without multi-timestep enhancements only
- v2 is the network with said enhancements and the baseline network

## To Install

- Install the following Python packages via the pip package manager (with the general form 'pip install \[package\]'):

  - tensorflow (unlike older versions, this will auto-install GPU compatibility and all dependencies)
  - pandas
  - numpy
  - cv2
  - matplotlib
  - scipy
  - scikit-learn

- (Optional) Install CUDA. This requires making a CUDA developer account on https://developer.nvidia.com/cuda-downloads and downloading the following installation:

    - CUDA v10.1
    
    Instructions at: https://docs.nvidia.com/cuda/
    
    Then, download and extract the following file into the CUDA v10.1 bin folder (on Windows 10, this will be C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.1\bin):
    
    - cudnn74_7.dll

- Install Jupyter Notebook. If the pip package manage is installed, run 'pip install notebook'. Other installation options can be found at: https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html

## To Run

- Download both the "Whisker Predictive Network" files. v1 is the code for the Baseline LSTM and Whisker Predictive Network with single timesteps. v2 also contains the Baseline LSTM, but the Whisker Predictive Network has been modified to use multiple timesteps.

- Run Jupyter Notebook via Command Prompt (Windows) or Terminal (Linux or Mac), with the command 'jupyter notebook'.

- Jupyter should load automatically. If it doesn't, copy and paste the link provided by the terminal output. This may require granting permissions to Jupyter via the browser. Tested to work on Google Chrome and Microsoft Edge.

- Find the desired file and open it in Jupyter. They will load Jupyter Notebooks and reside in their own tabs. Though not usually a problem, it is recommended to only load one file at a time, as some state is shared between instances despite the best efforts of the author.

- Download and unpack the data files from the link given in the Dissertation PDF, Appendix D

- Modify the filepath parameter of all instances of sio.loadmat() to point towards the 200805-Whiskerdata folder.

- Run all cells via Cells -> Run All. To ensure a run with no carryover of state, for subsequent runs use Kernel -> Restart and Run All
