# Changing permissions
To give access to all files and directories in my work space to my group:

To find directories and grant everyone in my group read write and execute permissions to directories 

    find -type d -exec chmod g+rwx {} \;

To find directories and grant everyone in my group read write and execute permissions to files

    find -type f -exec chmod g+rw {} \;

- find -type f \ #find all my files from current directory
- -exec \ #then execute the following
- chmod g+rw \ # change permissions to group gets read write
- {} \; #put what you found in here
