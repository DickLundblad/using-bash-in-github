# using-bash-in-github
run bash script in github
used for debugging bash scripts
## first task would be to create bash script for extracting specific commit messages
     git log --pretty=format:"%s"  | grep -oE "AB#[0-9]{6}+" | sort -u
## Extract commit messsage , from and to  Release Tags
    git log --pretty=format:"%s" "v1.0.0".."v1.1.2" | grep -oE "AB#[0-9]{6}+" | sort -u
