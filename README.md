
# linux-commands

- Remove everything ctrl+u
- Cut left word ctrl+w
- Reverse history search ctrl+r(> for edit, return to run)
- Check which Linux flavor (distribution + version)
  ```sh
  cat /etc/os-release
  ```
- Most recently sort files and folder
  ```sh
  ls -lt
  ```
- Least recently sort files and folder
  ```sh
  ls -ltr
  ```
- Listing lnclude hidden files
  ```sh
  ls -alt
  ```
- Filter filenames and runs them as arguments to ls -lt
  ```sh
  grep -ril "user" . | xargs ls -lt
  ```
- ### Find filename(.,~) with number list(nl)
  ```sh
 find . -name '*create*.sh' | nl
  ```
- Find location of file name If file is in your $PATH
  ```sh
  which ./create-aws-user.sh
  ```
- Use quotes for copy(source or destination full path)
  ```sh
  cp "/Users/neetupal/Downloads/project 2/secrets-setup.sh" .
  ```
- This prints the absolute (full) path
  ```sh
  readlink -f DevSetup.ps1
  ```
### Create group
```
sudo groupadd <group_name>
```
### Create user
```
sudo useradd -m <username>
```
### copy from local to remote
```
scp -i "D:\keypair.pem" rough.txt ubuntu@54.197.12.113:/home/ubuntu
```
### If the folder new is inside your current working directory
```
scp -i '/d/keypair.pem' -r new ubuntu@54.197.12.113:/home/ubuntu/
```
