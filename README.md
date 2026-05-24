# Nhom_7_Khoa_Hoc_Du_Lieu
# Hướng dẫn chạy notebook và script

## Mục đích

Thư mục này chứa:

* `batdongsan.ipynb` : notebook để phân tích dữ liệu bất động sản
* `batdongsan_vietnam1.csv` : dữ liệu đầu vào
* `run_nb.py` : script Python tùy chọn để chạy notebook tự động

## Yêu cầu

* Python 3.8+ hoặc tương đương
* Virtual environment `.venv` đã được cài đặt và kích hoạt
* Các gói cần thiết cho notebook (ví dụ: `pandas`, `matplotlib`, `seaborn`)

## Cách chạy trong VS Code

1. Mở thư mục này trong VS Code.
2. Mở file `batdongsan.ipynb`.
3. Chọn kernel Python từ `.venv` nếu VS Code chưa tự động chọn.
4. Chạy từng cell hoặc chọn `Run All` từ thanh công cụ notebook.

## Chạy trực tiếp bằng terminal

1. Mở terminal trong thư mục dự án.
2. Kích hoạt môi trường ảo, cài đặt thư viện và chạy notebook bằng các câu lệnh dưới đây:

```bash
# ---- BƯỚC 1: KÍCH HOẠT VIRTUAL ENVIRONMENT ----
# Nếu dùng PowerShell:
.\.venv\Scripts\Activate.ps1
# Nếu dùng Command Prompt (CMD):
.\.venv\Scripts\activate.bat

# ---- BƯỚC 2: CÀI CÁC GÓI CẦN THIẾT ----
pip install jupyter pandas matplotlib seaborn

# ---- BƯỚC 3: CHẠY NOTEBOOK ----
# Cách 3a: Chạy trực tiếp bằng nbconvert
python -m nbconvert --to notebook --execute batdongsan.ipynb --inplace

# Cách 3b: Hoặc mở giao diện Jupyter Notebook trên trình duyệt
python -m notebook
