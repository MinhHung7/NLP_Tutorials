# Text Representation
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/78cca7ea-e48a-479c-8211-13c9d469fca5)
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/60a752af-2430-4d0b-b367-f084cfab133f)
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/8533c045-667a-445f-8a97-40f3e5cf3ad8)
## Label Encoding
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/c7244628-a993-48cf-b04e-da21123a4a39)
## Bag Of Words (BOW)
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/7efb96e6-ab9e-4668-bcaf-bf738178e939)
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/309c8e16-e0dc-4f0e-ad6b-5dd997b798dc)
## Bag Of n-group
Giữa các từ trong một câu có một sự liên hệ với nhau.  
Có các trường hợp chỉ cần đổi chỗ 2 từ câu sẽ trở thành nghĩa khác  
Vd:  
Minh Hung sat on a **sofa** and ate a **samosa**  
Minh Hung sat on a **samosa** and ate a **sofa**  
- Nghĩa của một câu được xác định bằng thứ tự các từ
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/42b93bd5-1513-4f0c-841b-faf92e4fa009)
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/ae9628e3-ed02-44da-a07d-eaa81c33812c)
### Limitations of bag of n-grams model
- Nếu n tăng thì số chiều và độ loãng của model sẽ tăng
- Không thể giải quyết vấn đề vượt quá từ vựng (out of vocalbulary)
## TF_IDF
- Trong một đoạn văn bản ngoài các keywords dùng để phân loại chúng thì các từ chung chung khác (hay từ nhiễu) xuất hiện rất nhiều lần.
- Giả sử có article khác nhau nhưng số lượng từ nhiễu này của 2 đoạn văn bản lại có số lần xuất hiện khá tương tự nhau. Điều này làm cho máy tính nghĩ rằng 2 đoạn văn bản này như nhau.
### Chỉ số ảnh hưởng
- Sử dụng chỉ số ảnh hưởng để chỉ rõ mức độ ảnh hưởng của các từ nhiễu và keywords
***
**Document Frequency (DF)** = Number of times term t is present in all docs
***
![image](https://github.com/MinhHung7/NLP_Tutorials/assets/118424791/50b72eea-1e55-4ade-9454-7349532593dd)
***
**TF(t, d)** = Total Number of time term t is present in doc A / Total number of tokens in doc A  
**IDF(t)** = log(Total Documents / Number of documents term t is present in all docs)  
**TF - IDF** = TF(t, d) * IDF(t)
***
