In real-world software projects, giving full access to our files and directories represents a huge risk of having any malicious cracker or entity uploading a devious file or modifying a current file to execute code. 

Following our CMS example, `777` permissions mean that anyone will have complete control over your CMS, including having your database information and password.

### Finding secure file permissions

Even though the permissions system is not very wide (it only has 3 static numbers), files and directories often need different access for the server and the user to read, write or execute the files. 

For example, the `.htaccess` file is one of the files that is accessed by the _owner_ of the process running the server. So if you set the permissions too low, then your server won't be able to access the file and will cause an error. Therein lies the method to find the most secure settings. __Start too restrictive and increase the permissions until it works__.