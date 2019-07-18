# my-userful-bash
Some bash command I created or learned to make my life a bit easier. Still learning bash :D

1. List directory contents use long listing foramt.
```bash
alias l='ls -l'
```

2. When you pulling from master and your company is using Rails...
```bash
alias installStuff='yarn install && bundle install && bin/rails db:migrate RAILS_ENV=development'
```

3. Show public ip
```bash
function showMyPublicIp() {
  myip="$(dig +short myip.opendns.com @resolver1.opendns.com)"
  echo "My WAN/Public IP address: ${myip}"
}
```

4. Just too lazy to type haha...
```bash
alias gpom='git pull origin master'
```

5. Clear all local branch except master
```bash
alias clearbranch='git branch | grep -v "master" | xargs git branch -D'
```
