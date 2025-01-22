# Git 跟 GitHub 基本使用

## commit
- Hello!! Here is Luce. 
- I'm learning how to use github and git @home in 2025/1/21. 
- It's kinda sad becuz I started to learn this sh!t @ 20 almost 21 QAQ.
- I love coding so I started to learn Py and c.
- Maybe someday I can be an IT grl ~~~

---

## **正常使用流程**
clone -> branch -> add -> ✨code✨ -> commit -> push

> 記得新增 `.gitignore`，避免將不必要的檔案（例如配置檔案或虛擬環境）推送到遠端倉庫。

---

## **初始化指令**
1. **新增 README 檔案**  
    ```bash
    echo "# 專案名稱" >> README.md
2. **初始化 Git 倉庫**  
移動到資料夾後執行：  
    ```bash
    git init
3. **新增檔案到暫存區並提交**  
    ```bash
    git add README.md 
    git commit -m "Initial commit"
4. **設定分支為 `main` 並連結遠端倉庫**  
    ```bash
    git branch -M main 
    git remote add origin 專案連結 
    git push -u origin main

> 如果專案已經有遠端倉庫，直接 `clone`，無需重複初始化。

---

## **登入指令**
首次使用需要設定全域使用者資訊（只需設定一次）：  
    ```bash
    git config --global user.name "你的名稱" 
    git config --global user.email "你的電子郵件"

---

## **日常操作**
1. **加入追蹤和提交檔案**  
    ```bash
    git add . 
    git commit -m "描述修改內容"

2. **建立主分支**  
    ```bash
    git branch -M main

3. **新增並切換到新分支**  
    ```bash
    git checkout -b feature/your-feature-name

4. **推送分支到遠端倉庫**  
    ```bash
    git push -u origin 支線

> 若推送到 `main`，請確認更改無誤：
git push -u origin main

5. **更新主分支（拉取最新代碼）**  
    ```bash
    git pull origin main

---

## **下載專案**
從遠端倉庫複製專案到本地端：  
    git clone 專案連結

---

## **常用指令**
- **查看狀態**  
    ```bash
    git status
- **查看提交日誌**  
    ```bash
    git log
- **查看分支**  
    ```bash
    git branch
- **切換分支**  
    ```bash
    git checkout 支線名稱

---

## **Tips**
1. 如果倉庫為私有且使用 SSH，需要先設定 SSH 金鑰，然後遠端連結指令改為：
    ```bash  
    git remote set-url origin git@github.com:LuceZi/your-repo-name.git

2. 若多次修改快速提交與推送，可以執行以下命令：
    ```bash
    git add . 
    git commit -m "描述修改內容" 
    git push

---

**Have a nice day!** 😄  
_Luce_
