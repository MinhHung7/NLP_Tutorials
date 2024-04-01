# Naive Bayes Classifier
## Lời mở đầu
**Naive Bayes Classiffier** là một chủ đề quan trọng trong lĩnh vực Machine Learning. Thuật toán này không chỉ là một trong những công cụ phổ biến nhất trong phân loại văn bản và phân tích dữ liệu, mà còn là một trong những cơ sở quan trọng để hiểu về các thuật toán học máy phức tạp hơn.  

Naive Bayes Classifier dựa trên nguyên tắc cơ bản của Bayes, một trong những công cụ toán học mạnh mẽ nhất trong thống kê và xác suất. Tuy nhiên, dù mang tính đơn giản, nhưng Naive Bayes vẫn mang lại những kết quả ấn tượng và thường được sử dụng trong các ứng dụng thực tế từ phân loại email cho đến phát hiện thị trường tài chính.

## Phân loại
**Bernoulli Naive Bayes**: Thuật toán này giả sử tất cả các thuộc tính của dữ liệu là **nhị phân** (0, 1) . 0 biểu diễn rằng "Từ đó không xuất hiện trong document" và 1 biểu diễn rằng "Từ đó xuất hiện trong document"  

**Multinomial Naive Bayes**: Thuật toán này được sử dụng khi chúng ta có dữ liệu rời rạc (vd đánh giá một bộ phim từ 1-5 sao và mỗi lần đánh giá sẽ có tần suất xuất hiện). Trong việc học văn bản ta có số lượng của mỗi từ để có thể dự đoán hoặc đánh nhãn

**Gaussian Naive Bayes**: Bởi vì giả định với phân phối chuẩn, Gaussian Naive Bayes thường được sử dụng trong các trường hợp khi mà tất cả các thuộc tính của dữ liệu là liên tục **continuous**.

## Sklearn CountVectorizer
Trong lĩnh vực xử lý ngôn ngữ tự nhiên và học máy, việc biểu diễn văn bản dưới dạng các vector số là một bước quan trọng để có thể áp dụng các thuật toán học máy. Sklearn CountVectorizer là một trong những công cụ phổ biến nhất được sử dụng để chuyển đổi văn bản thành các vector số dễ dàng để làm việc.  

Sklearn CountVectorizer là một phần của thư viện Python scikit-learn (sklearn), được sử dụng để biểu diễn văn bản dưới dạng các vector số. Nó chuyển đổi một tập hợp các văn bản thành một ma trận, trong đó mỗi hàng của ma trận tương ứng với một văn bản, và mỗi cột tương ứng với một từ trong tập từ điển của các văn bản.

![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/63c642b8-49d6-45f8-a155-75737da341ce)


## Thực hành
Sử dụng datasets spam.csv để áp dụng thuật toán vào phân loại email liệu rằng một email có là spam hay không
