# FLINT Installation Guide

## Introduction
This guide provides detailed instructions for installing FLINT (Flexible Land-Use INTegration) on your local system. FLINT is an open-source land-use modeling platform developed by moja global.

---

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [VCPKG Installation](#vcpkg-installation)
3. [FLINT Installation](#flint-installation)
4. [Flint.example Installation](#flint-example-installation)
5. [Instructions for Chapmans Richards Example](#instructions-for-chapmans-richards-example)
6. [Setup Docker Container](#setup-docker-container)

---

## 1. Prerequisites <a name="prerequisites"></a>
Before installing FLINT, ensure you have the following prerequisites installed on your system:
- GitHub
- Visual Studio
- CMake
- Docker

---

## 2. VCPKG Installation <a name="vcpkg-installation"></a>
### 2.1. Cloning VCPKG Repository
1. Open GitHub and navigate to the moja-global repository.
2. Search for the VCPKG repository.
3. Copy the URL of the VCPKG repository: [https://github.com/moja-global/vcpkg.git](https://github.com/moja-global/vcpkg.git).
4. Create a folder named "Development" on your local desktop.
5. Within the "Development" folder, create a sub-folder named "moja-global".
6. Open the command prompt and navigate to the "moja-global" directory.
7. Clone the VCPKG repository using the following command:
    ```
    git clone https://github.com/moja-global/vcpkg.git
    ```

### 2.2. Installing VCPKG Packages
1. Navigate to the VCPKG directory in the command prompt.
2. Bootstrap VCPKG using:
    ```
    bootstrap-vcpkg.bat
    ```
3. Install required packages using:
    ```
    vcpkg.exe install [package1] [package2] ...
    ```
   Replace `[package1]`, `[package2]`, etc., with the required package names.

---

## 3. FLINT Installation <a name="flint-installation"></a>
### 3.1. Cloning FLINT Repository
1. Navigate to the moja-global repository on GitHub.
2. Copy the URL of the FLINT repository: [https://github.com/moja-global/FLINT.git](https://github.com/moja-global/FLINT.git).
3. In the command prompt, navigate to the "moja-global" directory.
4. Clone the FLINT repository using:
    ```
    git clone https://github.com/moja-global/FLINT.git
    ```

### 3.2. Building the FLINT Project
1. Switch to the develop branch of the FLINT repository.
2. Navigate to the FLINT folder and open a command prompt.
3. Create a build folder under the "source" folder.
4. Generate the Visual Studio Solution using CMake.

---

## 4. Flint.example Installation <a name="flint-example-installation"></a>
### 4.1. Cloning Flint.example Repository
1. Navigate to the moja-global repository on GitHub.
2. Copy the URL of the Flint.example repository: [https://github.com/moja-global/FLINT.Example.git](https://github.com/moja-global/FLINT.Example.git).
3. In the command prompt, navigate to the "moja-global" directory.
4. Clone the Flint.example repository using:
    ```
    git clone https://github.com/moja-global/FLINT.Example.git
    ```

### 4.2. Building Flint.example
1. Navigate to the Flint.example directory in the command prompt.
2. Create a build folder under the "source" folder.
3. Generate the Visual Studio Solution using CMake.

---

## 5. Instructions for Chapmans Richards Example <a name="instructions-for-chapmans-richards-example"></a>
### 5.1. Setting up Chapmans Richards Example
1. Navigate to the Flint.example folder in the moja-global directory.
2. Open the Visual Studio solution.
3. Set up the necessary configurations for running the Chapmans Richards example.

---

## 6. Setup Docker Container <a name="setup-docker-container"></a>
### 6.1. Building using Prebuilt Image
1. Pull the pre-built Docker image for FLINT from the moja-global GitHub Container Registry.
2. Run a container using the pulled image.
3. Verify the installation by running the CLI.

---


