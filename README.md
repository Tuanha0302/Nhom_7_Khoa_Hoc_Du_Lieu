# Nhom_7_Khoa_Hoc_Du_Lieu
# Hướng dẫn chạy notebook và script
# Link Youtube: https://youtu.be/Wffa7-w9uEE?si=rSzSiN1xcD5eOpqE
# Link Slide: https://www.canva.com/design/DAHKcmfVKxI/JAnwsQfnNMCsIy1_KD8Y5g/edit
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
2. Kích hoạt virtual environment (Chọn lệnh phù hợp với Terminal cậu đang dùng)

   Nếu dùng Command Prompt (CMD) / DOS:
   ```
   .\.venv\Scripts\activate.bat
   ```
   Nếu dùng PowerShell:
   ```
    .\.venv\Scripts\Activate.ps1
   ```
3. Cài các gói cần thiết nếu cần:
   ```
   pip install jupyter pandas matplotlib seaborn
   ```
4. Chạy trực tiếp notebook bằng nbconvert:
   ```
   python -m nbconvert --to notebook --execute batdongsan.ipynb --inplace
   ```
5. Hoặc mở Jupyter Notebook trực tiếp:
   ```
   python -m notebook#
   ```
### Ghi chú
- File run_nb.py là tùy chọn và không bắt buộc để chạy batdongsan.ipynb.

- Nếu notebook sử dụng đường dẫn tương đối, đảm bảo batdongsan_vietnam1.csv nằm trong cùng thư mục.

- Nếu notebook cần thư viện bổ sung, cài thêm với pip install .
