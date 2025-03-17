
---

# **Cat Lovers Website Project**

Welcome to the **Cat Lovers Website Project**! This project is designed to help you practice your HTML, CSS, and JavaScript skills while learning how to use Git and GitHub effectively. You'll also get familiar with Gitflow, a branching model for managing workflows in Git.

---

## **Project Overview**

This is a simple website about cats, with the following pages:
- **Home**: Introduction to cats and the website.
- **Good Practices**: Tips for taking care of cats.
- **Feed Tips**: Advice on feeding your cat.
- **Toys Tips**: Recommendations for cat toys.
- **Cats Habits**: Common behaviors of cats.
- **Contact**: A form to get in touch with us.

---

## **Repository URL**
[https://github.com/hackthegap/github-cats-website.git](https://github.com/hackthegap/github-cats-website.git)

---

## **Setup Instructions**

### **1. Clone the Repository**
To get started, clone the repository to your local machine using the following command:

```bash
git clone https://github.com/hackthegap/github-cats-website.git
```

### **2. Navigate to the Project Folder**
Move into the project directory:

```bash
cd github-cats-website
```

### **3. Open the Project**
You can open the project in your favorite code editor (e.g., VS Code):

```bash
code .
```

---

## **Basic Git Commands**

Here are some basic Git commands you'll use during this project:

### **1. Check the Status of Your Repository**
```bash
git status
```

### **2. Add Files to the Staging Area**
To stage all changes:
```bash
git add .
```

To stage a specific file:
```bash
git add <filename>
```

### **3. Commit Your Changes**
```bash
git commit -m "Your commit message here"
```

### **4. Push Changes to GitHub**
```bash
git push origin <branch-name>
```

### **5. Pull the Latest Changes from GitHub**
```bash
git pull origin <branch-name>
```

### **6. Create a New Branch**
```bash
git checkout -b <branch-name>
```

### **7. Switch to an Existing Branch**
```bash
git checkout <branch-name>
```

### **8. Merge Branches**
First, switch to the branch you want to merge into (e.g., `main`):
```bash
git checkout main
```

Then, merge the feature branch:
```bash
git merge <branch-name>
```

---

## **Gitflow Workflow**

Gitflow is a branching model for managing workflows in Git. Here's how you can use it in this project:

### **1. Main Branches**
- **`main`**: The production-ready branch. Always stable.
- **`develop`**: The branch for ongoing development.

### **2. Feature Branches**
- Create a new branch for each feature or task:
  ```bash
  git checkout -b feature/<feature-name>
  ```
- Work on your feature and commit changes:
  ```bash
  git add .
  git commit -m "Add <feature-name>"
  ```
- Push the feature branch to GitHub:
  ```bash
  git push origin feature/<feature-name>
  ```
- Merge the feature branch into `develop` when done:
  ```bash
  git checkout develop
  git merge feature/<feature-name>
  ```

### **3. Release Branches**
- When `develop` is ready for a release, create a release branch:
  ```bash
  git checkout -b release/<version>
  ```
- Merge the release branch into `main` and tag the release:
  ```bash
  git checkout main
  git merge release/<version>
  git tag -a v1.0 -m "Release version 1.0"
  ```

### **4. Hotfix Branches**
- For urgent fixes, create a hotfix branch from `main`:
  ```bash
  git checkout -b hotfix/<hotfix-name>
  ```
- Merge the hotfix into `main` and `develop`:
  ```bash
  git checkout main
  git merge hotfix/<hotfix-name>
  git checkout develop
  git merge hotfix/<hotfix-name>
  ```

---

## **Project Structure**

```
cat-website/
│
├── index.html              (Home Page)
├── good-practices.html     (Good Practices Page)
├── feed-tips.html          (Feed Tips Page)
├── toys-tips.html          (Toys Tips Page)
├── cats-habits.html        (Cats Habits Page)
├── contact.html            (Contact Form Page)
├── styles/
│   └── style.css           (CSS File)
├── scripts/
│   └── script.js           (JavaScript File)
└── images/                 (Folder for Images)
```

---

## **How to Contribute**

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Open a pull request to the `develop` branch of the main repository.

---

## **Credits**

- Images: [Unsplash](https://unsplash.com/) and [Pexels](https://www.pexels.com/).
- Instructor: Fabricio Braga & Holly Drazenovich

---

Happy coding! 🐾