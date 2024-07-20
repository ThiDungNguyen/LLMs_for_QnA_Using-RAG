#LLMs - RAG 

Large Language Models (LLMs) are advanced models that allow users to input text with any content, often in the form of requests or questions. These models then return a textual response that satisfies the user's request. Popular applications of LLMs include ChatGPT, Gemini, and other similar technologies.

RAG(Retrieval Augmented Generation) là một kỹ thuật giúp LLMs cải thiện chất lượng kết quả tạo sinh bằng cách tích hợp nội dung truy vấn được từ một nguồn tài liệu nào đó để trả lời cho một câu hỏi đầu vào. Trong project này, chúng ta sẽ tìm hiểu cách xây dựng một chương trình RAG cơ bản. Đồng thời, ứng dụng chương trình vào việc hỏi đáp tài liệu bài học trong khóa AIO. Theo đó, Input và Output của chương trình là:

• Input: File tài liệu cần hỏi đáp và một câu hỏi liên quan đến nội dung tài liệu.

• Output: Câu trả lời.


## Note 

- Tài liệu ( ảnh, âm thanh, video ..) được mã hoá dưới dạng vector database bằng embedding module. Từ vector data base, user có thể quẻy trên vector database, kết quả trả về sẽ là các vector có liên quan đến câu hỏi.
- embedding: đổi dạng text dang dạng số để máy tính có thể hiểu dễ nhất, và số dưới dạng vector sẽ dễ xử lý sau này nhất. sau đó so sánh sự tương đồng giữ vector prompting và vectors trong vector database. 
- hugging face used to call modules
- Langchain: cung cấp các hàm để hỗ trợ build các ứng dụng sử dụng LLMs. Langchain sẽ có các hàm trợ giúp như load files ( PDF, HTML, code, youtibe, axiv, notion, github ...) 
- phải có text splitter: vì câu trả lời cho 1 promting thường chỉ ở trong khoảng 2-3 dòng. nên nêú để cả 1 trang giấy dứoi dạng string of text, thì độ chính xác sẽ không được cao.
- chainlit: tương tự như streamlit, dùng để build app, nhưng chainlit chỉ dùng cho build chatbot.


## Installation
1. Clone the repository:
```sh
git clone https://github.com/ThiDungNguyen/LLMs_for_QnA_Using-RAG.git
cd LLMs_for_QnA_Using-RAG
```
2. (Optional) Create and activate a virtual environment:
```sh
python3 -m venv .pytorch
source .pytorch/bin/activate
```
3. Install the required dependencies:
```sh
pip install -r requirements.txt
```

## Run the application
```sh
python main.py
```
