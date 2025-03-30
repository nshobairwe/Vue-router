# vue-router tutorial steps

### 1. vue router setup project

### 2. router links

### 3. folder structure

### 4. router parameter

### 5. dynaminc links

### 6. redirect & 404

### 7. paragmatic navigation

# JSON SERVER SETUP steps

### 1. setup db.json file
### 2. install json server

### **Fix: Install `json-server`**  

#### **1. Install `json-server` Globally**  
Run this command:  
```sh
npm install -g json-server
```

#### **2. Verify Installation**  
Check if `json-server` is installed:  
```sh
json-server --version
```
If the version number appears, you're good to go.

#### **3. Run `json-server`**  
```sh
json-server --watch data/db.json
```

---

### **Alternative: Use Local Installation**
If you prefer a local installation (inside the project), run:
```sh
npm install json-server
```
Then start it using:
```sh
npx json-server --watch data/db.json
```

Let me know if you still face issues! 🚀
