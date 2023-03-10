# Notifier
Receive notifications on your phone when your CLI tasks complete.

**sleep 3; notifier "Sleep task completed."**

**rsync -avz . philippe@my-server:"/media/philippe/"; notifier "Rsync done."**

<p align="center"><img src="show.jpg" width="25%"></img></p>

- Download the Alertzy app to receive the notifications on your iPhone.
- Save the Alertzy key in your bashrc/zshrc: `export ALERTZY_KEY="blabla"`

Download the script
```bash
wget https://raw.githubusercontent.com/philipperemy/notifier/master/notifier && chmod +x notifier
```

Test it
```bash
sleep 3 && notifier "Sleep task done"
```

Install it
```bash
mkdir ~/bin && cp notifier ~/bin
export PATH="~/bin:$PATH" # add it to your bashrc/zshrc.
notifier "OK"
```
