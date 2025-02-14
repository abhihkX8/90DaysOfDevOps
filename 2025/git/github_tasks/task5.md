========== This is my fifth task ============


### **Exploring SSH Authentication in GitHub**  

SSH authentication allows you to securely connect to your GitHub repository without needing to enter your username and password every time. Here’s how to set it up:  

---

### **Step 1: Check for an Existing SSH Key**  
Before generating a new SSH key, check if you already have one:  

```bash
ls -al ~/.ssh
```
If you see files like `id_rsa.pub` or `id_ed25519.pub`, you already have an SSH key. You can use that or generate a new one.

---

### **Step 2: Generate a New SSH Key**  
If you don’t have an SSH key or want to create a new one, run:  

```bash
ssh-keygen 
```


### **Step 3: Add Your SSH Key to GitHub**  
Copy your SSH public key to your clipboard:  

```bash
cat ~/.ssh/id_ed25519.pub
```
OR  
```bash
cat ~/.ssh/id_rsa.pub
```
1. Go to **GitHub → Settings → SSH and GPG Keys**  
   ([Direct Link](https://github.com/settings/keys))  
2. Click **"New SSH Key"**  
3. Paste your public key and save it.

---

### **Step 4: Test SSH Connection**  
Verify that SSH authentication is working:  

```bash
ssh -T git@github.com
```
If successful, you’ll see:  
> *Hi `<your-username>`! You've successfully authenticated, but GitHub does not provide shell access.*

---

### **Step 5: Change Git Remote to SSH**  
Switch your repository’s remote URL from HTTPS to SSH:  

```bash
git remote set-url origin git@github.com:<your-username>/90DaysOfDevOps.git
```
To check if it was updated successfully:  

```bash
git remote -v
```

---

### **Step 6: Push Your Code Using SSH**  
Now, push your branch securely via SSH:  

```bash
git push origin feature-update
```

---

### **🎉 You’re Now Using SSH Authentication!**  
