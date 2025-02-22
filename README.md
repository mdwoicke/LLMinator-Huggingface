## LLMinator: Run & Test LLMs locally

#### Gradio based tool with integrated chatbot to locally run & test LLMs directly from HuggingFace.

An easy-to-use tool made with Gradio, LangChain, and Torch.

![LLMinator chat tab](https://github.com/Aesthisia/LLMinator/assets/89995648/0c7fd00f-610b-4ad1-8736-1f0cb7d212de)
![LLMinator models tab](https://github.com/Aesthisia/LLMinator/assets/89995648/44c03281-fb76-40c6-b1d3-2e395562ae16)

### ⚡ Features

- Context-aware Chatbot.
- Inbuilt code syntax highlighting.
- Load any LLM repo directly from HuggingFace.
- Supports both CPU & CUDA modes.
- Enable LLM inference with [llama.cpp](https://github.com/ggerganov/llama.cpp) using [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)

## 🚀 How to use

To use LLMinator, follow these simple steps:

- Clone the LLMinator repository from GitHub.
- Navigate to the directory containing the cloned repository.
- Install the required dependencies by running `pip install -r requirements.txt`.
- Build LLMinator with llama.cpp :

  - Using `make`:

    - On Linux or MacOS:

      ```bash
      make
      ```

    - On Windows:

      1. Download the latest fortran version of [w64devkit](https://github.com/skeeto/w64devkit/releases).
      2. Extract `w64devkit` on your pc.
      3. Run `w64devkit.exe`.
      4. Use the `cd` command to reach the `LLMinator` folder.
      5. From here you can run:
         ```bash
         make
         ```

  - Using `CMake`:
    ```bash
    mkdir build
    cd build
    cmake ..
    ```

- Run the LLMinator tool using the command `python webui.py`.
- Access the web interface by opening the provided URL in your browser.
- Start interacting with the chatbot and experimenting with LLMs!

### Command line arguments

| Argument Command | Default   | Description                                                                 |
| ---------------- | --------- | --------------------------------------------------------------------------- |
| --host           | 127.0.0.1 | Host or IP address on which the server will listen for incoming connections |
| --port           | 7860      | Launch gradio with given server port                                        |
| --share          | False     | This generates a public shareable link that you can send to anybody         |

## Installation and Development Tips

**Python Version:**

- **Compatible Versions:** This project is compatible with Python versions 3.8+ to 3.11. Ensure you have one of these versions installed on your system. You can check your Python version by running `python --version` or `python3 --version` in your terminal.

**Cmake and C Compiler:**

- **Cmake Dependency:** If you plan to build the project using Cmake, make sure you have Cmake installed.
- **C Compiler:** Additionally, you'll need a C compiler such as GCC. These are typically included with most Linux distributions. You can check this by running `gcc --version` in your terminal. Installation instructions for your specific operating system can be found online.

**Visual Studio Code:**

- **Visual Studio Installer:** If you're using Visual Studio Code for development, you'll need the C++ development workload installed. You can achieve this through the [Visual Studio Installer](https://visualstudio.microsoft.com/vs/features/cplusplus/)

**GPU Acceleration (CUDA):**

- **CUDA Installation:** To leverage GPU acceleration, you'll need CUDA installed on your system. Download instructions are available on the [NVIDIA website](https://developer.nvidia.com/cuda-toolkit).
- **Torch Compatibility:** After installing CUDA, confirm CUDA availability with `torch.cuda.is_available()`. When using a GPU, ensure you follow the project's specific `llama-cpp-python` installation configuration for CUDA support.

## Reporting Issues:

If you encounter any errors or issues, feel free to file a detailed report in the project's repository. We're always happy to help! When reporting an issue, please provide as much information as possible, including the error message, logs, the steps you took, and your system configuration. This makes it easier for us to diagnose and fix the problem quickly.

## 🤝 Contributions

We welcome contributions from the community to enhance LLMinator further. If you'd like to contribute, please follow these guidelines:

- Fork the LLMinator repository on GitHub.
- Create a new branch for your feature or bug fix.
- Test your changes thoroughly.
- Submit a pull request, providing a clear description of the changes you've made.

Reach out to us: info@aesthisia.com