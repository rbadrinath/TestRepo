This is a test repository
I first logged on to my github account and created a TestRepo project
How I created this:
On my local machine I have already been using git
$ mkdir testrepo ; cd testrepo
$ git init
# This next step was needed to make sure some stuff worked on my VM, I dont think it is really needed 
$ git config --global --add safe.directory /media/sf_courses/<directory_name like testrepo>
# Then I edited a little README.md file
$ git add README.md
$ git commit -m 'First commit'
$ git branch -M main
# Rest was as indicated by gihub when I created the TestRepo project :
$ git remote add origin git@github.com:rbadrinath/FCP.git
$ git push -u origin main
