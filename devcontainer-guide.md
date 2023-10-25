# How to create a devcontainer with VSCode?

## Steps to follow

1. Create a github repo for your project.
2. Create a project directory.
3. Open the directory in VSCode.
4. Make sure the required extensions are installed.
5. Initialise git.
6. Press `Ctrl+Shift+P`, search and select
   `Dev Containers: Add Dev Container Configuration Files`.
7. Choose what programming lanuages, OSs or other features to install, and
   VSCode will create a `devcontainer.json`.
8. Before reopening the project in the container, add a few lines to the newly
   created `devcontainer.json`.
9. Copy and paste the following code to the `devcontainer.json` file:

   ```json
   "mounts": [
      "type=bind,source=/home/${localEnv:USER}/.ssh,target=/root/.ssh,readonly"
   ]
   ```

   By pasting these lines to the file, we can now push code to Github
   (Admittedly, there must be a better way to do this. Suggestion: go read the
   *Sharing Git credentials with your container* VSCode guide listed in the
   resources section)

10. Now, reopen your project in the container by pressing `Ctrl+Shift+P` and
    run

## Online resources I used to create this guide

1. [Is there a way to get git to work properly from within a dev container using VS Code?](https://stackoverflow.com/questions/60495428/is-there-a-way-to-get-git-to-work-properly-from-within-a-dev-container-using-vs)
2. [Share SSH keys with VS Code Devcontainer running with Docker's WSL2 backend](https://stackoverflow.com/questions/70206554/share-ssh-keys-with-vs-code-devcontainer-running-with-dockers-wsl2-backend)
3. [Sharing Git credentials with your container](https://code.visualstudio.com/remote/advancedcontainers/sharing-git-credentials)
