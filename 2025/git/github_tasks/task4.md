 ========= This is my forth Task ===========


### **Task 5: Advanced Branching and Switching**  

Branching allows you to work on different features or bug fixes without affecting the main codebase.  

---

### **Step 1: Create a New Branch**  
To create a new branch, run:  

```sh
git branch feature-branch
```
This creates a new branch called `feature-branch` but doesn’t switch to it yet.  

---

### **Step 2: Switch to the New Branch**  
To switch to your new branch:  

```sh
git checkout feature-branch
```
OR (modern method using `switch`):  

```sh
git switch feature-branch
```

Now, any changes you make will be on `feature-branch`, not `main`.  

---

### **Step 3: Make Changes and Commit**  
Edit or create files, then add and commit changes:  

```sh
git add .
git commit -m "Added new feature"
```

---

### **Step 4: Merge Branch into Main**  
Once your feature is ready, switch back to `main` and merge:  

```sh
git checkout main
git merge feature-branch
```
OR using `switch`:  

```sh
git switch main
git merge feature-branch
```

---



### 🎉 **Now you have mastered advanced branching!**  


### **Modify the File and Commit Changes**  

Follow these steps to update `info.txt` and push your changes to GitHub.

---

### **Step 1: Edit `info.txt`**  
Open `info.txt` in a text editor and make changes. If using the command line, you can add text with:  

```sh
    vim  info.txt
```

---

### **Step 2: Stage the Changes**  
After editing the file, stage it:  

```sh
git add info.txt
```

---

### **Step 3: Commit the Changes**  
Commit with a descriptive message:  

```sh
git commit -m "Feature update: Enhance info.txt with additional details"
```

---

### **Step 4: Push to Remote Repository**  
Ensure you're on the correct branch (`feature-update`), then push the changes:  

```sh
git push origin feature-update
```

---

### 🎉 **Your file update is now in GitHub!**  





