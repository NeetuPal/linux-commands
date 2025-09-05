# linux_command_cheatSheet

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
- Find filename
  ```sh
  find . -name *create*.sh
  ```
- Find location of file name
  ```sh
  which ./create-aws-user.sh
  ```
- Use quotes for copy(source or destination full path)
  ```sh
  cp "/Users/neetupal/Downloads/project 2/secrets-setup.sh" .
  ```
