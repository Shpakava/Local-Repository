mkdir local
git init
cd local
nano File.txt
git add .
git commit –m ‘new File.txt’
git push - -set -upstream Local_Repository master
git fetch
git branch develop
git checkout develop
git branch develop1
git checkout develop1
nano File.txt
git add File.txt
git commit –m ‘new File.txt on develop1’
git push - -set -upstream Local_Repository develop1
git checkout develop
git branch develop2
git checkout develop2
nano File.txt
git add File.txt
git commit –m ‘new File.txt on develop2’
git push - -set -upstream Local_Repository develop2
git checkout develop
git push - -set -upstream Local_Repository develop
git merge develop1
git merge develop2
CONFLICT
nano File.txt
git add .
git commit –m ‘conflict resolved’
