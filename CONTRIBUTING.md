# Contributing to this project

Thanks to contributing.

## Rules

Có 1 vài quy tắc đơn giản để bất kì ai viết dự án có thể thực hiện, và nên thực hiện (bởi vì tôi sẽ rất buồn đấy nếu như bạn không làm theo :D).

### KHÔNG git push lên main branch

Quy tắc tối thiểu mà bạn cần làm theo khi đóng góp trong dự án này, đó là KHÔNG được đẩy code lên nhánh main.

Thay vào đó, hãy tạo một nhánh khác, đặt tên theo cú pháp `[name]-[feature]` với `[name]` là tên bạn và `[feature]` (không bắt buộc) là tên tính năng bạn đang phát triển.

Để tạo nhánh mới, dùng `git switch -c [branch]` với `[branch]` là tên nhánh mới (mà tôi đã đề cập bên trên ấy) hoặc là `git switch [branch]` nếu nhánh đã tồn tại. 

Nhớ nhé, KHÔNG `git push origin main`.

## Báo cáo lỗi

Một báo cáo lỗi tốt là một báo cáo lỗi chứa:

- Expected behavior (hành vi mong muốn)
- Actual behavior (hành vi đã xảy ra)
- Exact reproduction steps (các bước thực hiện hành vi lỗi)
- Frequency (tần suất xuất hiện: `always`, `sometimes` hay `once`).
- Environment details (chi tiết môi trường sử dụng), bao gồm:
    - OS + version (ví dụ như Windows 22h2).
    - Phiên bản của chương trình dự án.
- Logs (đại khái là bằng chứng lỗi, ví dụ như ảnh chụp màn hình).

Báo cáo lỗi có thể là lỗi logic, lỗi hiệu năng, hoặc bất kể lỗi nào tuân theo quy tắc `hành vi xảy ra không đáp ứng kì vọng`.

## Commits

Các git commits cần theo message-rules sau để giúp những người khác hiểu rõ bạn đã làm gì:

`[tag]:[verbs][dirs][details]`

Trong đó: 

- `[tag]`: có thể là tên nhánh (branch), tên tag (tag release), tên phiên bản (version).
- `[verbs]`: add, edit, delete, fix
- `[dirs]`: tên folders hoặc files mà `[verbs]` ảnh hưởng đến
- `[details]`: chi tiết việc đã làm (viết ngắn gọn, và có thể bỏ nếu thấy không cần thiết)

Ví dụ:

`First commit: init, add & edit docs/`

`JustRubik: fix #123 (to free my mind)`

*\#123 là mã của issue* 

