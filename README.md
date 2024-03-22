# Whisper Transcriber

## Overview
This project utilizes HuggingFace transformers to make it possible for you to chat with your LLM models that are available open-source.

## Getting Started

### Prerequisites
Ensure you have Python installed on your system. This project has been set up and tested using the configurations,guidelines and features provided by the HuggingFace. The python version used is 3.10.

### Installation
1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies using the following command:

```
pip install -r requirements.txt
```
**Note:**  Its recommened by the Huggingface page to install flash attention via the following
```
pip install flash-attn --no-build-isolation
```

**Note for macOS Users:** During installation, you may encounter issues with NVIDIA CUDA-related packages and `bitsandbytes`. These packages are not supported on macOS and should be commented out in the `requirements.txt` file before proceeding with the installation.

### Configuration
All configurations can be implemented in the `app.py` file (since I am a noob to streamlit but I like its interface). This includes changing the model by updating the `model_id` to use a model that you would like.
A word of caution, please only use models which can be utilized by your system. Do refer to memory requirements of the desired model you want to run.

### Running the Application
To start the app, use the following command:

```
streamlit run app.py 
```


## Support
For more detailed information about configurations and usage, refer [here](https://huggingface.co/docs/transformers/v4.39.0/en/index).

## Contributing
I welcome contributions! Please feel free to submit pull requests or open issues to improve the project or fix problems.