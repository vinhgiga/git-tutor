# Hướng dẫn nhanh về GitHub

## Tạo tài khoản GitHub

[Hướng dẫn tạo tài khoản GitHub](https://learn.microsoft.com/en-us/visualstudio/version-control/git-create-github-account?view=vs-2022)

## Cài đặt Git

- Bạn có thể tải installer file từ trang web: <https://git-scm.com/downloads>
- Với Windows có thể cài đặt thông qua command-line installer [scoop](https://scoop.sh/). Chạy các lệnh sau trên Windows PowerShell:

    1. Cài đặt scoop:

        ```shell
        Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
        irm get.scoop.sh | iex
        ```

    2. Cài đặt Git:

        ```shell
        scoop install git               # install git
        scoop cache rm *                # remove all installer files
        ```

## Cấu hình Git

Bạn có thể cấu hình git bằng cách chạy các lệnh sau:

```shell
git config --global user.name "user name"
git config --global user.email "user@MailServer"
git config --global credential.helper manager-core
```

## Tạo Repository (Kho lưu trữ)

[Tài liệu hướng dẫn tạo Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

## Upload code lên GitHub

Sau khi bạn tạo một Repository mới, GitHub sẽ hiển thị hướng dẫn nhanh các lệnh để đẩy code lên GitHub. Dưới đây là các bước đẩy code từ một project đã tồn tại trên máy:

1. Điều hướng đến thư mục chứa project
2. Mở thư mục project với Terminal
3. Chạy các lệnh sau trên Terminal

```shell
git init
git add .
git commmit -m "first commit"
git remote add origin https://github.com/username/repo-name.git
git push -u origin master
```
them moi'''


