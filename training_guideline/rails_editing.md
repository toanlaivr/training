# Hướng dẫn học Rails Tutorial

## 1. Mục tiêu
Phần này sẽ hướng dẫn cho các bạn cách phát triển một ứng dụng web sử dụng framework RubyonRails. Rails Tutorial được xây dưng để cung cấp cho bạn sự giới thiệu đầy đủ về cách phát triển ứng dụng web, bao gồm nền tảng cơ sở trong Ruby, Rails, HTML & CSS, databases, version control, testing, and deploy ứng dụng. Nếu bạn đã biết phát triển web, khóa học này sẽ nhanh chóng dạy cho bạn các yếu tố cần thiết của framework RubyOnRails, bao gồm MVC và REST, generators, migrations, routing, and embedded Ruby.
Vào cuối khóa học này, sinh viên sẽ có thể:
  - Biết cách cài đặt và cấu hình Ruby, Rails và những package liên quan
  - Hiểu về vòng đời một request trong Rails
  - Ứng dụng kiến trúc Model-View-Controller cho các ứng dụng phía máy chủ
  - Học lập trình các thành phần chính của Rails, bao gồm Active Record, Action Controller và Action View
  - Tìm hiểu các nguyên tắc cơ bản của Ruby
  - Xây dựng các ứng dụng hướng dữ liệu với Rails
  - Thực hiện TDD (test-driven development) cho các ứng dụng Rails.
  - Hoàn thành một ứng dụng blog với những chức năng cơ bản.

## 2. Thời gian học:
9 ngày

## 3. Link tài liệu:
- Các bạn đọc và làm theo cuốn Rails 6 - Tutorial theo link (Bỏ phần Test, k đẩy lên git phần test): [Rails Tutorial](https://drive.google.com/drive/folders/1y6xUxiFsuI3Qyx53yajYUcvRDJINPpUN)
- Tham khảo bản dịch Tutorial bằng tiếng Việt: [Bản dịch Tutorial](https://docs.google.com/document/d/1cRZAH6hnrTVDEdceAKrG1eynz_EHoFoB/edit?rtpof=true)

- Nội dung cần tự học và trả lời sau mỗi chương: [Link](https://docs.google.com/spreadsheets/d/1S306g-Z6DWjkaJyMEkoZUJXZrdB5iLpVopARi9AdO4M/edit?usp=sharing)

## 4. Về việc gửi pull request
Pull đầu tiên sẽ là init_project.Các bạn lên github tạo 1 repo mới chọn Initialize this repository with a README, add .gitignore chọn Ruby => Tạo repo, Sau đó clone về máy. Sau đó
```
git checkout -b init_project
rails new .
git add .
git commit -m "Init Project"
git push origin init_project
```
Rồi kiểm tra trên git tạo 1 pull request mới, đọc hướng dẫn bên dưới để trainer có thể review pull.

Từ chapter 3 -> chapter 14. Sau mỗi chapter, các bạn thực hiện tạo pull request để gửi trainer review.

#### Yêu cầu:
- Mỗi 1 pull request tương ứng 1 chapter
- Cách đặt tên:
  + Tên repo github là: **sample_app**
  + Tên branch tương ứng với tên chapter. Ví dụ: **chapter_3**, **chapter_4**
  + Tiêu đề pull request (nội dung commit): Tiêu đề của chapter đó.
    Ví dụ: "Chapter 3: Mostly static pages", "Chapter 6: Modeling users"

## 5. Thiết lập IDE
Sublime Text
Các bạn sử dụng setting này dành cho sublime để xử lý indent, trailing space và end of file, bằng cách:
Preference -> Setting User -> xóa hết cái cũ và paste đoạn code sau vào:
```yaml
{
  "ensure_newline_at_eof_on_save": true,
  "font_size": 14,
  "highlight_line": true,
  "ignored_packages":
  [
    "Vintage"
  ],
  "rulers":
  [
    80
  ],
  "show_encoding": true,
  "show_line_endings": true,
  "tab_size": 2,
  "translate_tabs_to_spaces": true,
  "trim_trailing_white_space_on_save": true,
  "binary_file_patterns":
  [
    ".bundle/",
    "bin/",
    "log/",
    "tmp/",
    "test/",
    "vendor/assets/fonts/"
  ],
  "draw_minimap_border": true,
  "update_check": false,
  "word_wrap": true
}
```

VS code
```yaml
{
    "explorer.confirmDelete": false,
    "editor.tabSize": 2,
    "explorer.confirmDragAndDrop": false,
    "files.trimTrailingWhitespace": true,
    "files.insertFinalNewline": true,
    "files.trimFinalNewlines": true,
    "workbench.startupEditor": "newUntitledFile",
    "window.zoomLevel": 0,
    "workbench.colorTheme": "Atom One Dark",
    "javascript.format.enable": false,
    "javascript.format.insertSpaceAfterCommaDelimiter": false,
    "javascript.format.insertSpaceAfterConstructor": false,
    "[ruby]": {
        "editor.formatOnSave": false
    },
    "workbench.iconTheme": "vscode-great-icons"
}
```
## 6. Một số lưu ý trong quá trình làm tutorial:
- Tuyệt đối không chờ đợi merged pull request chapter trước rồi mới làm chapter tiếp theo. Thay vào đó, các bạn checkout branch mới từ branch trước ra và làm tiếp, sau này sẽ rebase và fix conflict sau nếu có.
- Pull request sau khi gửi trainer, các bạn chờ đợi trong thời gian tối đa là 3 tiếng, nếu sau 3 tiếng vẫn chưa có người review, các bạn hãy gửi message nhắc nhở trainer trên Mattermost.
- Nên để 1 commit/pull trong quá trình học tutorial.
- Trong quá trình làm nếu gặp vấn đề không giải quyết được thì hãy chủ động hỏi nhờ các bạn khác hoặc Trainer để được support.

## 7. Coding convention
Các bạn self review code của cá nhân theo coding convention của công ty theo link sau:
https://github.com/framgia/coding-standards/blob/master/vn/README.md

## 8. Bài test:
Host: http://training.sun-asterisk.vn
