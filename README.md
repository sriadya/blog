# tensorflow
tensorflow notebooks

Git refference
For first time commit
1. git config --global user.name "Your Name"
2. git config --global user.email "youremail@domain.com"

Create a new Repo (tensorflow in this case)

3. git clone (url)
4. git add (file names)
5. git commit -m "(committed message)
6. git push -u origin master
Git has a 100Mb file size limit. I had initially commited the pickle as well. The push failed because of the file size.
To remove the file from commit used the following command
7.  git filter-branch --index-filter 'git rm --cached --ignore-unmatch notMNIST.pickle'

To create a new remote

8. git remote add origin master (url) 

   git remote add pybook https://github.com/adyagit/pybooks.git

Push Conflicts

9. If push Updates were rejected because the remote contains work that you do not have locally, 

   git pull  - will solve the conflict. Its not suggested to do a --force push
