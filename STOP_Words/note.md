# STOP Words
## Vấn đề
Ở bài học trước, ta biết rằng từ một đoạn tài liệu hay văn bản, ta có thể gắn nhãn cho đoạn văn bản đó
bằng cách sử dụng phương pháp BOWs (Bag Of Words).  
Thế nhưng ngoài các keywords liên quan tới nhãn của mình thì cũng có những từ làm nhiễu khác xuất hiện trong văn bản (ex. to, for, over, ...) và chúng xuất hiện với tần suất rất nhiều.  
Do vậy ta không thể xác định xem nhãn đúng là cái gì  
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/305515eb-c952-42d3-8b9f-f95cf2b7d744)
Nên nếu ta có thể loại bỏ các từ nhiễu này, phương pháp BOWs sẽ trở nên tốt hơn
## Khi nào không nên loại bỏ từ nhiễu
**This is a good movie -> good movie**  
**This is not a good movie -> good movie**  
