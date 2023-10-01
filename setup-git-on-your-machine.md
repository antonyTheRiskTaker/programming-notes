How to set up git on your machine?
(Source: https://kbroman.org/github_tutorial/pages/first_time.html)
1. Get a github account.
2. Download and install git.
3. Set up git with your user name and email.
   i. Run `git config --global user.name "Your name here"`
   ii. Run `git config --global user.email "your_email@example.com"`
4. Set up ssh on your computer.
   i. Look to see if you have files ~/.ssh/id_rsa and ~/.ssh/id_rsa.pub.
      If not, create such public/private keys: `ssh-keygen -t rsa -C "your_email@example.com"`
   ii. Copy your public key into your clipboard.
5. Paste your ssh public key into your github account settings.
   i. Go to your github Account Settings.
   ii. Click “SSH Keys” on the left.
   iii. Click “Add SSH Key” on the right.
   iv. Add a label (like “My laptop”) and paste the public key into the big 
       text box.
   v. In a terminal/shell, type the following to test it: 
      `ssh -T git@github.com`. If it says something like the following, it 
      worked: "Hi username! You've successfully authenticated, 
      but Github does not provide shell access."