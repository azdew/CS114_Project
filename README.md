# Đồ án CS114

## Cấu trúc thư mục mẫu
<pre><code>
├── classification
│   ├── khoa
│   │   └── dataset1
│   │       ├── info.txt
│   │       └── model1
│   │           ├── info.txt
|   |           ├── result.csv
|   |           ├── best_model.pth
|   |           └── score.txt
│   └── nhan
│       └── dataset1
│           ├── info.txt
│           └── model1
│               ├── info.txt
|               ├── result.csv
|               ├── best_model.pth
|               └── score.txt
└── linear_regression
    ├── khang
    │   └── dataset1
    │       ├── info.txt
    │       └── model1
    │           ├── info.txt
    |           ├── result.csv
    |           ├── best_model.pth
    |           └── score.txt
    └── kien
        └── dataset1
            ├── info.txt
            └── model1
                ├── info.txt
                ├── result.csv
                ├── best_model.pth
                └── score.txt
</code></pre>

## Quy ước
- Mỗi người làm việc trong thư mục của mình.
- Khi thay đổi dataset thì người đó tự tạo thêm thư mục `dataset2`, `dataset3`,...
- Model nào liên quan tới dataset nào thì nằm trong thư mục `datasetpth` đó (cách đặt tên tương tự như đặt tên cho dataset)
- File `info.txt` trong thư mục `dataset` và `model` chính là file để ghi thông tin về dataset hoặc model đó (ví dụ model này thay đổi learning_rate = 1e^-3, model kia đổi kích thước ảnh thành x*x,...)
- Vậy thư mục `model` gồm 5 file:
  - `info.txt`: như đã nói ở trên
  - `result.csv`: là file kết quả đã nộp lên wecode
  - `score.txt`: là file lưu lại điểm số tương ứng với file `results.csv` đã nộp
  - `best_model.pth`: là file tham số model tốt nhất được lưu từ hàm torch.save(...)
  - `[id bài nộp].ipynb`: là file code model tương ứng cho ra `result.csv` và `best_model.pth`
