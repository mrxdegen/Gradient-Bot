# **Gradient Network Bot**
<br><br><br>

## **Owerview**

- **Getting Started**: [User Guide](https://jammers-organization.gitbook.io/gradient-network-bot-or-jambit-x-mr.-x)  
- **Installation**: [Installation Guide](https://jammers-organization.gitbook.io/gradient-network-bot-or-jambit-x-mr.-x/installation-guide)  
- **Interface**: [Interface Owerview](https://jammers-organization.gitbook.io/gradient-network-bot-or-jambit-x-mr.-x/interface-overview)  

## **Purchase Information**

- **Price**: $150  

## **System Requirements**

- **Operating System**: Windows/Linux (Ubuntu 22.04)  
- **Internet Connection**: Required  
- **Additional Requirements**:  
  - Valid email accounts for registration  
  - Proxy configurations (if applicable)  

---

## **Instructions for running Gradient Network Bot on Ubuntu 22.04**

### **1. Create a Working Folder for the Bot**
Run the following command to create a working directory:  
```bash
mkdir /home/gradient-example-bot
```

### **2. Transfer Files**
Use an FTP/SFTP client to transfer the **Linux executable file** and the **`.env` file** (containing your secret data and settings) to the working directory:  
`/home/gradient-example-bot`  

### **3. Run the Bot in a Screen Session**  
Screen ensures the bot continues running even if the terminal session is closed.

1. **Navigate to your working folder**:  
   ```bash
   cd /home/gradient-example-bot
   ```

2. **Create a screen session**:  
   ```bash
   screen -S gradient-bot-session
   ```

3. **Run the bot**:  
   ```bash
   ./gradientbot-v-1.1.5
   ```

4. **Detach the screen session** (leave the session running):  
   Press `Ctrl + A`, then `D`.

### **4. Other Useful Commands**
- **To delete a session**:  
  ```bash
  screen -X -S gradient-bot-session quit
  ```
- **To re-enter a session**:  
  ```bash
  screen -r gradient-bot-session
  ```
- **To view all active sessions**:  
  ```bash
  screen -ls
  ```

### **5. Troubleshooting**
- If you encounter a **permission denied error**, run the following command before starting the bot:  
  ```bash
  chmod +x /home/gradient-example-bot/gradientbot-v-1.1.5
  ```