This is a test repository.

I am documenting how I created this:

1. I first logged on to my github account and created a TestRepo project

1. On my local machine that I have already been using git  
$ mkdir testrepo ; cd testrepo  
$ git init

1. This next step was needed to make sure some stuff worked on my VM, I dont think it is really needed  
$ git config --global --add safe.directory /media/sf_courses/<directory_name like testrepo>

1. Then I edited a little README.md file, and then added it to the local repo...  
$ git add README.md  
$ git commit -m 'First commit'  
$ git branch -M main

1. Rest was as indicated by gihub when I created the TestRepo project :  
$ git remote add origin git@github.com:rbadrinath/FCP.git  
$ git push -u origin main

1. A note on the .git/config in the project directory:  
I found it was important to have this in there:
~~~text
[remote "origin"]
	url = git@github.com:rbadrinath/TestRepo.git
~~~
Also make sure to configure the global .gitconfig file with email and name set.

