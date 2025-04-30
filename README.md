# **CMDProtector**  
_A multi-functional program designed to enhance server security using OTP authentication, PIN management, and administrative owner options._  

---

## **About CMDProtector**  

CMDProtector is an advanced utility program for managing server security, user authentication, and administrative functionalities. It is compatible with both **Windows Server** and **Linux Server**, providing cross-platform capabilities and support for OTP tokens and PIN-based authentication.  

---

## **Features**  

- **Secure Authentication**: Use OTP tokens or PINs for access.  
- **Owner Options**: Admin-only controls for managing access, clearing data, and viewing IP/location.  
- **Cross-Platform Support**: Works seamlessly on Windows and Linux systems.  
- **Easy Setup**: Automatic initialization and integration into server environments.  

---

## **Installation and Setup**  

### **Windows Server Setup**  

1. **Install Python**  
   - Download Python from [Microsoft Store](https://apps.microsoft.com/store/) or [python.org](https://www.python.org/downloads/).  
   - Check the box for **Add Python to PATH** during installation.  
   - Verify Python installation by running:  
     ```bash
     python --version
     ```

2. **Download CMDProtector**  
   - Navigate to the release page: [CMDProtector Release - SERVER.V1](https://github.com/DaniDemaDD/CMDProtector/releases/tag/SERVER.V1).  
   - Download the ZIP file from **Assets** and extract it to a folder on the server.

3. **Install Required Libraries**  
   - Open the Command Prompt (`Win + R`, type `cmd`, press Enter).  
   - Navigate to the folder where the files are extracted:  
     ```bash
     cd path\to\folder
     ```  
   - Run:  
     ```bash
     python install_requirements.py
     ```

4. **Generate OTP Token**  
   - Go to the `GENERATETOKEN` folder.  
   - Open the terminal inside this directory (right-click → Open in Terminal).  
   - Run the script to generate the token:  
     ```bash
     python auth_qr_terminal.py
     ```

5. **Integrate into the System**  
   - Double-click on `INSTALL_AUTORUN.bat` to integrate CMDProtector into the system.  

6. **Run the Program**  
   - Launch the program by opening `run.bat`. Follow the menu to use CMDProtector.

---

### **Linux Server Setup**  

1. **Install Python**  
   - Open the terminal and run the following commands to install Python 3 and pip:  
     ```bash
     sudo apt update
     sudo apt install python3 python3-pip -y
     ```

2. **Download CMDProtector**  
   - Directly download the release ZIP file from the GitHub page:  
     ```bash
     wget https://github.com/DaniDemaDD/CMDProtector/releases/download/SERVER.V1/CMDProtector.zip
     ```  
   - Extract the ZIP file:  
     ```bash
     unzip CMDProtector.zip
     cd CMDProtector
     ```

3. **Install Required Libraries**  
   - Install all dependencies using:  
     ```bash
     python3 install_requirements.py
     ```

4. **Generate OTP Token**  
   - Navigate to the `GENERATETOKEN` directory:  
     ```bash
     cd GENERATETOKEN
     ```  
   - Run the script:  
     ```bash
     python3 auth_qr_terminal.py
     ```  

5. **Run CMDProtector**  
   - Return to the main folder and start the program:  
     ```bash
     python3 cmd_block.py
     ```  
   - Use the program’s menu for authentication and owner functionalities.

---

## **Important Notes**  

- Ensure all files remain in their original structure after extraction to maintain functionality.  
- CMDProtector is built for **Windows Servers** but works on **Linux Servers** with minor adjustments.  
- For Linux Servers without GUI, commands like opening URLs (`os.system("start URL")`) will not work.  

---

## **License**  

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).  
