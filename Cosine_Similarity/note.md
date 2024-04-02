# Cosine Similarity
## Đặt vấn đề
Giả sử bạn đang làm việc cho một công ty quản lý tài chính.  
Công ty của bạn có một kho Drive chứa rất nhiều các tài liệu liên quan.  
Nhưng bạn lại không biết những công ty nào liên quan tới mỗi tài liệu trong Drive.  
Nhưng nếu bạn mở một tài liệu ra và đọc nó, bạn có thể dễ dàng biết được công ty nào đang liên quan.  
**Giả sử**  
Một tập tài liệu có liên quan tới Apple Inc có nội dung như sau:  
___
**iPhone** sales contributed to 70% of revenue.  
**iPhone** demand is increasing by 20% yoy.  
The main competitor phone **Galaxy** recorded 5% less growth compared to **iPhone**
___  
Bạn có thể đoán được công ty Apple có liên quan tới tài liệu này hơn là Samsung. Đơn giản là vì tỷ lệ xuất hiện của từ iPhone nhiều hơn Galaxy  
| Thành phần | Số lượng |
|------------|---------|
| iPhone     | 3       |
| Galaxy     | 1       |

Một ví dụ khác cho thấy công ty Samsung có liên quan tới tài liệu:  
___
Samsung Electronics unveils its **Galaxy** S21 flagship, with modest spec improvements and a significantly lower price point.  
**Galaxy** S21 price is lower by ~20% (much like the **iPhone** 12A), ... Samsung's focus on **Galaxy** redesign...boosting shipments of **Galaxy**  
___
| Thành phần | Số lượng |
|------------|---------|
| iPhone     | 1       |
| Galaxy     | 4       |

## Vector hóa
Mọi thứ ta có thể đưa về dạng vector như sau  
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/b017aa88-9489-46ee-94ea-0110bfc21938)

Biểu diễn trên đồ thị, ta được:  
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/b085291c-46a0-44bb-b279-66042fa27508)

## Cosine Similarity
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/e7d9e3bb-f061-4809-b807-dfdf6129fb70)

Với giá trị Cosine Similarity gần 1, có thể hiểu rằng 2 đoạn văn bản có nội dung tương tự nhau  
Ngược lại với giá trị Cosine Similarity gần 0  
## Cosine Distance
Cosine Distance = 1 - Cosine Similarity
