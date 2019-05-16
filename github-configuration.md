
# GitHub Configuration

`# setting up connection to github`

cd ~  `# change directory to your home directory`

ssh-keygen -t rsa -b 4096 "your.email@domain.com"

eval `ssh-agent -s`  `# not single quote - back tick`

ssh-add ~/.ssh/id_rsa  `# add the private key`

`# register with your public key`
`# these keys are located in ~/.ssh folder`
`# private key = rsa_id`
`# public key = rsa_id.pub`
`# upload public key to github --> settings --> ssh --> add ssh keys`
