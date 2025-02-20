

import os
import sys

# Data Labs - Instructions
1. Create a new repository in your personal GitHub account.
2. Complete assignments in Google Colab.
3. Upload your completed Google Colab notebook (`.ipynb` file) to the repository.
3. Copy the link to your repository.
4. Submit the link in [Canvas/Blackboard/Google Classroom].


### GitHub Guide for Students ###

## What is GitHub?
GitHub is a web-based platform that enables version control, collaboration, and project management for software development. It uses Git, a distributed version control system, to help track changes, manage branches, and collaborate on code.

## Key Features of GitHub:
1. **Repositories (Repos)** - Storage for code, files, and version history.
2. **Commits** - Save changes to a repository.
3. **Branches** - Create separate versions of a project for experimentation.
4. **Pull Requests (PRs)** - Suggest changes and merge branches.
5. **Issues** - Track bugs, feature requests, and improvements.
6. **GitHub Actions** - Automate workflows like testing and deployment.
7. **GitHub Classroom** - Manage assignments and submissions for students.

## Creating a New Project on GitHub
1. **Sign in to GitHub** at [GitHub](https://github.com/).
2. Click on the **"+"** button in the top right corner and select **"New repository"**.
3. Enter a repository name (e.g., `python-assignment-1`).
4. Choose **Public** or **Private** visibility.
5. Select **Initialize this repository with a README**.
6. Click **Create repository**.
7. Clone the repository locally using:
   ```bash
   git clone https://github.com/your-username/DataLab.git
   ```

## Linking an Existing Google Colab Project to GitHub
1. **Open Google Colab** at [Google Colab](https://colab.research.google.com/).
2. Open your notebook or create a new one.
3. Click **"File" → "Save a copy in GitHub"**.
4. Sign in to GitHub if prompted.
5. Select the repository where you want to save the file.
6. Add a commit message and click **"OK"**.

### Manually Pushing Google Colab Notebooks to GitHub
1. **Mount Google Drive** (if using Drive to store files):
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. **Download the Notebook**:
   ```python
   !wget -O my_notebook.ipynb "https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID"
   ```
3. **Push the Notebook to GitHub**:
   ```bash
   git clone https://github.com/your-username/python-assignment-1.git
   mv my_notebook.ipynb python-assignment-1/
   cd python-assignment-1
   git add my_notebook.ipynb
   git commit -m "Added assignment notebook"
   git push origin main
   ```

By following these steps, you can integrate your Google Colab assignments with GitHub for better version control and submission tracking.
