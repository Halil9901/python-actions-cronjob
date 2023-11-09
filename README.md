# Schedule a Python script with GitHub Actions
- Make sure you have enabled read and write for the actions to run successfully
  ```
  Repo Settings -> actions-> general -> Workflow permissions -> Readn and write permissions
  ```
- Make sure you keep the reqirements.txt updated when new packages are installed
 ```
pip3 freeze > requirements.txt  # Python3
pip freeze > requirements.txt  # Python2
```

- Implement your script in `main.py`
- Inspect and configure cron job in GitHub Action `.github/workflows/actions.yml`
- It can install and use third party packages from `requirements.txt`
- Secret environment variables can be used. Set secrets in Settings/Secrets/Actions -> 'New repository secret'. Use the same secret name inside `actions.yml` and `main.py`
