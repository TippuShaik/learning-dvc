# Version your data with DVC

## Softwares required (If you are using Google Drive as your backend storage).
$ pip install "dvc[gdrive]"** 

$ dvc --version

## Command to use:

***To initialize DVC in your repositories***
$ git init
$ dvc init 

***To Add your data to DVC***
$ dvc add ./data

***To Add your changes to Git***
$ git add data.dvc .gitignore (Adding your changes to Git)

***To Add your external storage to dvc***
$ dvc remote add -d gdrive gdrive://<storage-uri> 

***To check the status of dvc and git***
$ dvc status 
$ git status

***To commit the changes to git and dvc***
$ git commit "Changes"
$ dvc push

***If you want to revert the changes to previous version***
$ git log
$ git checkout <commit-id>
$ dvc pull
