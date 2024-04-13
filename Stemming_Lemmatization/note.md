# Stemming and Lemmatization
## Vấn đề
Khi chúng ta search một chủ đề nào đó trên các công cụ tìm kiếm như Google, Chrome, ... 
thì các công cụ sẽ tìm các từ khóa sao cho matchs với keyword có trong câu của chúng ta
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/f2c22759-be16-410a-b9ed-08e473c69ca6)

**talking** -> **talk**  
**eating** -> **talk**  
**ate** -> **eat**  
**adjustable** -> **adjust**  
Sử dụng các phương pháp như bỏ **able, ing, ...** để rút thành dạng cơ bản  
Nhưng đôi khi các phương pháp trên cũng không hiệu quả  
Ví dụ như để chuyển **ate -> eat**  
Nên chúng ta cần có các kiến thức về ngôn ngữ để dễ dàng hơn trong việc xử lý dạng rút gọn này  
**base word = lemmatization**  

