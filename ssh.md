SSH keys generation cheatsheet
=======
1. Create a new ssh key, using provided email ad a label:
	> ssh-keygen -t rsa -C "my_email@example.com"

2. Start the ssh-agent in the backgroud
	> eval 'ssh-agent -s'

3. Add the key to the ssh-agent
	> ssh-add ~/.ssh/id_rsa

4. Copy public key to clipboard and paste it in e.g. GitHub or wherever else...
	> pbcopy < ~/.ssh/id_rsa.pub

