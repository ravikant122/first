# commands

# clone
it used to download repo on your local machine
command -- git clone <link of your repo>

# status
gives status of repo
command -- git status

# add
it adds the files in repo
command -- git add .  (for all the files that are untracked means git don't know about these files)
command -- git add <file name>

# commit
it saves the changes locally means not the site(github.com)
command -- git commit -m "<msg>" -m "<description>"
use this to verify yourself -> git config --global user.email "ravikanttatiwal1999@gmail.com"

# to commit on the website -- we've to generate SSH key first
first create .ssh folder in c/users/hp, if not exists

ssh-keygen -t <crypto_algo_name(dsa/rsa)> -b <key_len(4096)> -C "<github email>"
for file name -- don't type anything -- just enter
for passphrase -- give anything that u can remember or enter(nothing)

two files will be generated -- id_rsa(private key file), id_rsa.pub(public key file)
open pub file using cat -- cat <directory/id_rsa.pub> 
copy its content
go to github ssh setting
go to add new ssh key, paste the copied content -- ssh key generated 

now link ssh key to ssh agent
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa    or   ssh-add (it will add default files)


