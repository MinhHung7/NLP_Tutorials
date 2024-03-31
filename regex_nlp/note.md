# Regex
Regex là một dạng tìm kiếm thông tin theo một mẫu **pattern** nào đó, được gọi là **matching patern**.  
Điều này có nghĩa khi bạn có một chuỗi thông tin nào đó, **regex** có thể giúp bạn rút trích thông tin, hay từ khóa từ chuỗi thông tin đó phục vụ cho mục đích người dùng.  
**Regex** là bài học quan trọng đầu tiên vì trong rất nhiều trường hợp, **Regex** có thể giúp bạn giải quyết các bài toán NLP mà không cần đến bất kì kiến thức gì về Machine Learning

## Regex trong giao dịch, mua sắm
Giả sử như bạn vừa đặt mua một món đồ nào đó qua mạng và gặp vài vấn đề với món đồ đó. Bạn sẽ làm gì?  
Chúng ta có thể lên trang web bán hàng của món đồ đó và thực hiện chat với chatbot của website đó 
***
**User**: Xin chào, tôi gặp vài vấn đề với **món đồ** đã mua 2 ngày trước. Mã của nó là **#12424525**  
**Chatbot**: Vâng, cảm ơn bạn đã liên hệ. Sau đây là thông tin của món đồ  
             -  **Mã**: #12424525  
             -  **Tên sản phẩm**:  Thuốc chống mất gốc lập trình  
             -  **Đơn giá**: 125$  
             -  **Ngày mua**: 31/03/2024  
             -  **Mã khách hàng**: KH005  
***
Có thể thấy rằng, chỉ với một chuỗi phản hồi từ user, chatbox có thể rút ra keys và thực hiện truy vấn để trả lời phù hợp cho user  
Ngoài ra, mặc dù user chat với các form khác nhau thì chatbox vẫn có thể trả lời hay giải đáp thắc mắc, chẳng hạn như:
***
**User**: **Món đồ** mã **#12424525** của tôi gặp vấn đề, xin hãy giúp đỡ  
**User**: Tôi đã mua **Món đồ** với giá 50$ mã là **#12424525**, hãy phản hồi giúp tôi  
...
***
Ngoài ra, Regex có thể áp dụng để kiểm số sđt, email, ...
## Regex trong kiểm tra sđt, email
Một cách đơn giản của regex, như là  
Với số điện thoại (123)-456-789, hay 123456789, ta có thể viết thành (xxx)-xxx-xxx, và xxxxxxxxx  
Với email abc@zyz.com, ta có thể viết thành xxx@xxx.com  
Dĩ nhiên, dạng regex này không hoàn toàn đúng, nhưng giúp hiểu rõ hơn về cách hoạt động của **regex**
## Sử dụng regex
Một vài trang web giúp support regex, trong đó là https://regex101.com/
Các key word cần chú ý sẽ được liệt kê trong bảng dưới đây:

| Meaning | Key |
| --------------- | --------------- |
| A single character of: a, b or c | [abc] |
| A character except: a, b or c | [^abc] |
| A character in range: a-z | [a-z] |
| A character not in the range: a-z | [^a-z] |
| A character in range a-z or A-Z | [a-zA-Z] |
| Any single character | . |
| Alternate - match either a or b | a \| b |
| Any whitespace character | \s |
| Any non-whitespace character | \S |
| Any digit | \d |
| Any non-digit | \D |
| Any word character | \w |
| Any non-word character | \W |
| Match everything enclosed | (?:...) |
| Capture everything enclosed | (...) |
| Zero or one of a | a? |
| Zero or more of a | a* |
| One or more of a | a+ |
| Exactly 3 of a | a{3} |
| 3 or more of a | a{3,} |
| Between 3 and 6 of a | a{3,6} |
| Start of string | ^ |
| End of string | $ |
| A word boundary | \b |
| Non-word boundary | \B |


Vd:
# Regex tutoria

```python
import re

chat1 = 'what the fuck going on with you: 123456789, hungm0235@gmail.com, 0739511556'
chat2 = 'my phone is (123)-456-789, hungm0235@gmail.com'
chat3 = 'my phone: 123456789, email: hungm0235@gmail.com'

pattern = '\d{9,10}|\(\d{3}\)-\d{3}-\d{3,4}'
matches = re.findall(pattern, chat3)
matches
```

```python
['123456789']

