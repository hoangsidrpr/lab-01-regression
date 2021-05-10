<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Forks][forks-shield]][forks-url]
[![Apache License][license-shield]][license-url]

Programming language: ![](https://img.shields.io/github/languages/count/nhutnamhcmus/lab-01-regression?style=flat-square) with ![](https://img.shields.io/github/languages/top/nhutnamhcmus/lab-01-regression?style=flat-square)

Open project with Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nhutnamhcmus/lab-01-regression/blob/main/source_code/introduction_to_machine_learning_project_01_regression.ipynb)

# ĐỒ ÁN THỰC HÀNH 01 - HỒI QUY

Lớp: Nhập môn Học Máy - CQ2018/21
Năm: 2021

## Bài toán

Chi phí sử dụng dịch vụ y tế là bài toán nhằm xác định các yếu tố ảnh hưởng đến
số tiền mỗi cá nhân phải chi trả cho hoạt động y tế cá nhân để từ đó dự đoán chi
phí sử dụng y tế của 1 người dựa trên các yếu tố đã thu thập. Cụ thể, sinh viên
được cung cấp 2 tập tin “train.csv” và “test.csv” chứa thông tin y tế cá nhân tại Mỹ
được thu thập dựa trên các thông tin được thu thập sau:
- **Age**: Tuổi
- **Sex**: Giới tính
- **BMI**: Chỉ số khối cơ thể
- **Children**: Số lượng trẻ con/người phụ thuộc
- **Smoker**: tình trạng hút thuốc
- **Region**: khu vực sinh sống
- **Charges**: Chi phí y tế cá nhân

## Yêu cầu

| #   | Nội dung                                                        |  Tình trạng 🔨 |
| --- | ---------------------------------------------------------------------------- | ------------ |
| 1   | Đọc và phân tích các đặc trưng trong 2 tập tin được cung cấp. Trình bày các thông tin hữu ích (insights) tác động đến chi phí y tế cá nhân.        |       Done   |
| 2   | Cài đặt các thuật toán máy học đã được học để dự đoán chi phí y tế cá nhân.       |       Done   |
| 3   | Báo cáo kết quả đạt được sau quá trình phân tích và cài đặt. Từ đó nhận xét về các tác nhân ảnh hưởng mạnh/yếu tới chi phí y tế cá nhân.       |       Done   |

## Đọc và phân tích các đặc trưng dữ liệu
- Đọc dữ liệu và kiểm tra dữ liệu
- Tiền xử lý dữ liệu
- Các đại lượng thống kê cơ bản của đặc trưng chi phí y tế
- Mối tương quan giữa các đặc trưng trong dữ liệu
- Phân tích đặc trưng chi phí y tế
- Phân tích mối quan hệ chi phí y tế (charges) - vùng (region)
- Phân tích mối quan hệ chi phí y tế - vùng - giới tính
- Phân tích mối quan hệ chi phí y tế - vùng - tình trạng hút thuốc
- Phân tích mối quan hệ chi phí y tế - vùng - số lượng trẻ con/ người phụ thuộc
- Phân tích mối quan hệ giữa chi phí y tế và tuổi nhóm theo tình trạng hút thuốc
- Phân tích mối quan hệ giữa chi phí y tế và chỉ số BMI nhóm theo tình trạng hút thuốc
- Phân tích mối quan hệ giữa chi phí y tế và số lượng trẻ con/ người phụ thuộc nhóm theo tình trạng hút thuốc

## Cài đặt các thuật toán máy học

### Sử dụng thuật toán Hồi quy Tuyến tính - Linear Regression
- Trình bày sơ lược Hồi quy Tuyến tính
- Các thức sử dụng, cài đặt bằng Sklearn thông qua thực hiện huấn luyện trên tập train.csv, test.csv
- Trực quan hóa kết quả 
- Nhận xét ưu điểm, nhược điểm của mô hình Hồi quy Tuyến tính

### Sử dụng thuật toán Hồi quy Ridge - Ridge Regression
- Trình bày sơ lược Hồi quy Ridge 
- Các thức chọn alpha tối ưu, sử dụng, cài đặt bằng Sklearn thông qua thực hiện huấn luyện trên tập train.csv, test.csv
- Trực quan hóa kết quả 
- Nhận xét ưu điểm, nhược điểm của mô hình Hồi quy Ridge 

### Sử dụng thuật toán Hồi quy Lasso - Lasso Regression
- Trình bày sơ lược Hồi quy Lasso
- Các thức chọn alpha tối ưu, sử dụng, cài đặt bằng Sklearn thông qua thực hiện huấn luyện trên tập train.csv, test.csv
- Trực quan hóa kết quả 
- Nhận xét ưu điểm, nhược điểm của mô hình Hồi quy Lasso

### Sử dụng thuật toán Random Forest Regressor
- Trình bày sơ lược Hồi quy Lasso
- Các thức sử dụng, cài đặt bằng Sklearn thông qua thực hiện huấn luyện trên tập train.csv, test.csv
- Đánh giá nhận định mức độ ảnh hưởng của các đặc trưng lên chi phí y tế cá nhân
- Trực quan hóa kết quả huấn luyện, kiểm tra trên tập test
- Nhận xét ưu điểm, nhược điểm của mô hình Hồi quy Rừng ngẫu nhiên - Random Forest Regressor

### Sử dụng thuật toán Polynomial Regression
- Trình bày sơ lược Hồi quy Đa thức
- Các thức chọn bậc đa thức tối ưu, sử dụng, cài đặt bằng Sklearn thông qua thực hiện huấn luyện trên tập train.csv, test.csv
- Trực quan hóa kết quả 
- Nhận xét ưu điểm, nhược điểm của mô hình Hồi quy Đa thức

## Các kết quả đạt được
- So sánh, nhận định các giải pháp lên bài toán
- Kiểm tra, đánh giá độ tốt của mô hình thông qua một số độ đo: MAE, RMSE, R2 Score

## Nhận xét/ Bình luận
- Lựa chọn mô hình thích hợp cho bài toán
- So sánh kết quả mô hình và kết quả dựa đoán trực quan hóa dữ liệu

## Đóng góp 

- Issue Tracker: github.com/nhutnamhcmus/lab-01-regression/issues
- Source Code: github.com/nhutnamhcmus/lab-01-regression

## Hỗ trợ/ Liên hệ

Mọi thông tin hỗ trợ hoặc liên hệ, xin vui lòng gửi trực tiếp về một trong các email dưới đây:

- Personal email: namle1232000@gmail.com

- Working email: lenam.fithcmus@gmail.com

- Student email: 18120061@student.hcmus.edu.vn

Hoặc tạo một github tracker ở mục Đóng góp

## Tham khảo
- [Machine Learning cơ bản - Bài 3: Linear Regression](https://machinelearningcoban.com/2016/12/28/linearregression/)
- [Random Forest Algorithm with Python and Scikit-Learn](https://stackabuse.com/random-forest-algorithm-with-python-and-scikit-learn/)
- [Random Forest Regression](https://levelup.gitconnected.com/random-forest-regression-209c0f354c84)
- [Sklearn document - Linear Model](https://scikit-learn.org/stable/modules/linear_model.html#)
- [Introduction to Linear Regression and Polynomial Regression](https://towardsdatascience.com/introduction-to-linear-regression-and-polynomial-regression-f8adc96f31cb)
- [Applied Data Mining and Statistical Learning - STAT 897D - PennState Eberly College of Science - Lesson 5: Regression Shrinkage Methods - Ridge Regression](https://online.stat.psu.edu/stat857/node/155/)
- [ML Hồi quy tuyến tính (Linear Regression) - Đỗ Minh Hải Blog](https://dominhhai.github.io/vi/2017/12/ml-linear-regression/)
- [arXiv: Lecture notes on ridge regression](https://arxiv.org/pdf/1509.09169;Lecture)
- [Applied Regression Analysis - STAT 897D - PennState Eberly College of Science - Lesson 7: Transformations \& Interactions - 7.7 - Polynomial Regression](https://online.stat.psu.edu/stat462/node/158/)

## Giấy phép

Đồ án/ tập tin báo cáo của mình sử dụng với giấy phép MIT LICENSE. Các tài liệu liên quan được dẫn liên kết tham khảo, citi trong file báo cáo và ghi rõ trong mục tham khảo, việc sử dụng các tài liệu này theo phần quy định của các tác giả.

## Lời cám ơn

Trong quá trình thực hiện đồ án này, chúng em đã nhận được rất nhiều sự giúp đỡ cũng như hỗ
trợ từ các thầy cô Trường Đại học Khoa học Tự nhiên, ĐHQG-HCM và các bạn bè trong lớp Nhập
môn Học Máy. Chúng em xin bày tỏ lòng cảm ơn chân thành đến mọi người vì đã giúp đỡ hướng dẫn,
chỉ bảo rất tận tình.

Đặc biệt, chúng em xin bày tỏ lòng biết ơn sâu sắc đến các thầy cô khoa Công nghệ Thông tin,
cụ thể hơn là thầy Bùi Tiến Lên và các thầy hướng dẫn đã giảng dạy rất nhiệt, cung cấp nhiều slides,
tài nguyên học tập cần thiết, tạo điều kiện tốt nhất để chúng em có thể hoàn thành được đồ án này.

Trong quá trình, viết báo cáo này, chúng em không thể tránh khỏi nhiều thiếu sót, hy vọng mong
nhận được góp ý từ thầy để chúng em tiếp tục hoàn thiện hơn đối với đồ án này, cũng như rút kinh
nghiệm cho những đồ án, những báo cáo kế tiếp.

Một lần nữa, cũng không cảm ơn đến gia đình, những người bạn, đã luôn đồng hành giúp đỡ lẫn nhau, để chúng mình có thể hoàn thành đồ án một cách hoàn chỉnh nhất có thể!

<!-- MARKDOWN LINKS & IMAGES -->

[contributors-shield]: https://img.shields.io/github/contributors/nhutnamhcmus/lab-01-regression?style=flat-square
[contributors-url]: https://github.com/nhutnamhcmus/lab-01-regression/graphs/contributors

[forks-shield]: https://img.shields.io/github/forks/nhutnamhcmus/lab-01-regression?style=flat-square
[forks-url]: https://github.com/nhutnamhcmus/lab-01-regression/network/members

[stars-shield]: https://img.shields.io/github/stars/nhutnamhcmus/lab-01-regression?style=flat-square
[stars-url]: https://github.com/nhutnamhcmus/lab-01-regression/stargazers

[license-shield]: https://img.shields.io/github/license/nhutnamhcmus/lab-01-regression?style=flat-square
[license-url]: https://github.com/nhutnamhcmus/lab-01-regression/blob/master/LICENSE
