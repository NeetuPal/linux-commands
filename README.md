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
- Find subdirectories included recursively(-nr for newest first option)
  ```sh
  find . -type f -exec stat -f "%m %N" {} \; | sort -n
  ```
