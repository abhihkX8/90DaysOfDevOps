 ============ This is My Third Task ==============


### **Task 3: Configure Remote URL with PAT and Push/Pull**  

To work with a remote repository, you'll need to:  
1. **Set the remote URL using a Personal Access Token (PAT)**  
2. **Push your local changes to GitHub**  
3. **Pull updates from GitHub**

---

### **Step 1: Set Up a Remote Repository with PAT**  
#### **Generate a Personal Access Token (PAT)**  
1. Go to [GitHub → Settings → Developer Settings → Personal Access Tokens](https://github.com/settings/tokens).  
2. Click **"Generate new token (classic)"** (or use fine-grained tokens for more security).  
3. Select scopes like `repo` (for private repos) and `workflow` (if needed).  
4. Copy the generated token (you won’t see it again).  

#### **Set the Remote URL Using the Token**  
Run the following command, replacing `your-username`, `your-repo`, and `your-token`:  

```sh
git remote add origin https://your-username:your-token@github.com/your-username/your-repo.git
```
To verify the remote URL:  
```sh
git remote -v
```

---

### **Step 2: Push Local Changes to GitHub**  
After configuring the remote, push your changes:  

```sh
git branch -M main  # Rename branch to main (if needed)
git push -u origin main
```
You'll be prompted for authentication if using HTTPS without a stored token.

---

### **Step 3: Pull Updates from GitHub**  
To fetch and merge the latest changes from the remote repository:  

```sh
git pull origin main
```

---

### 🎉 **Now your repository is linked with GitHub!**  




