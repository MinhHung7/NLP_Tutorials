# Tokenization
## Tokenization
- Sentence tokenization là quá trình xử lý tiền dữ liệu (pre-processing). Quá trình này thực hiện chia tách một đoạn văn bản thành các câu.  
- Word tokenization là quá trình xử lý tiền dữ liệu (pre-processing). Quá trình này thực hiện chia tách một câu thành các từ khóa (keys).  
- Nói chung **tokenization** là quá trình tách văn bản thành các segments
## Why do we need this library
Nếu bạn thực sự nghĩ mình có thể chia tách văn bản thành các thành phần nhỏ hơn dựa vào cách nhận biết
các dấu câu như (., !, ?, ...) thì bạn có thể mắc sai lầm   
***
Vd: "Dr. Strange ordered samosas, revioli etc. for his lunch  
Sentence #1: Dr  
Sentence #2: Strange ordered samosas, revioli etc  
Sentence #3: for his lunch  
***
