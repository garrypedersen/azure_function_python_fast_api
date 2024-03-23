# Azure Function : Python : FAST API
Running a Python FAST Api within an Azure Function.

I wanted to better understand how to use dev containers, Python Azure Fuctions, and FAST API.

# Project Structure
* .devcontainer
    * Contains defintions for running the dev container.
* function_app.py
    * Fuction logic entry point. Delegates calls to FastAPIApp/\_\_init\_\_.py.
* FastAIPApp\\_\_init\_\_.py
    * Contains FAST API logic.

# Running Locally

## Prerequisites
1. Visual Studio Code
2. Dev Containers Extension
3. Docker

## Steps
1. Clone the repo.
2. Open folder in VS Code.
3. Execute the command: ```Dev Containers: Open Folder in Container```
4. Once the container is built and running, ensure that the Azurite Local Storage extension is running. ```Azurite: Start``` will do the trick. 
5. Hit F5 / Run and Debug and the Azure Function should start up and listening for requests at http://localhost:7071. The dev container includes the Thunder Client extension you can use to issue requests against the API with. 
