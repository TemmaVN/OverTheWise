#Đây là write-up cho những bạn mới biết về linux
#Linux làm việc chủ yếu trên Terminal nên những bạn mới khó tiếp cận. Nên cần làm quen nhiều và thực hành.
#Link làm bài : https://overthewire.org/wargames/bandit/
##Bandit0
- Đề bài : 
![image](https://hackmd.io/_uploads/rJWMo0gyee.png)
- Bài này đơn giản chỉ cần dùng lệnh ssh kết nối cổng 2220 của bandit.labs.overthewire.org:
```
    ssh bandit0@bandit.labs.overthewire.org -p 2220
```
#Lưu ý mỗi bài ta cần kết nối với lệnh tương tự nhưng thay ```bandit0``` thành bài làm
#Ví dụ 
```
    ssh bandit1@bandit.labs.overthewire.org -p 2220
```
- Mật khẩu: ```bandit0``` (Đề cho) :+1: 
##Bandit0->1
- Đề bài : 
![image](https://hackmd.io/_uploads/H1LSnCgJxe.png)
![image](https://hackmd.io/_uploads/SkM6nReJxg.png)
- Ta dùng ```ls``` để hiển thị các file có trong folder hiện có và ``` cat ``` để đọc nội dung file (như mở word).
- Z là có mật khẩu: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
##Bandit1->2
- Đề bài:
![image](https://hackmd.io/_uploads/BkBRp0lJgx.png)
- Tương tự ta mở folder xem chứa gì ```ls```.
![image](https://hackmd.io/_uploads/rkSI0CgJxl.png)
- Ta đọc file bằng lệnh ```cat``` nhưng tên file chứa kí tự đặc biệt ```-``` nên khi gõ lệnh nó sẽ hiểu ta đang nhập lệnh.
- Nên cần thêm ```.\``` trước tên file để hiểu rằng là ta đang đọc file ```-``` , ```cat .\-```
![image](https://hackmd.io/_uploads/SJQPy1Z1ge.png)
- Mật khẩu: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
##Bandit2->3 (Dần hiểu rùi nên nội dung vắn tắt lại !!!)
- Đề bài:
![image](https://hackmd.io/_uploads/Hy0MlJWJeg.png)
- Dùng ```cat``` để đọc và do chứa khoảng cách nên dùng trong cặp dấu ```""``` 
- Nếu không sẽ hiểu đọc 4 file liên tiếp - sai.```cat "spaces in this filename"```
- Mật khẩu: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
##Bandit3->4
- Đề bài : 
![image](https://hackmd.io/_uploads/Skei71Zyll.png)
- Dùng lệnh ```cd inhere``` để mở folder nhưng có vấn đề! Nó rỗng
- Thay vì dùng ```ls``` ta dùng ```ls -la``` để mở tất cả kể cả chúng bị ẩn
![image](https://hackmd.io/_uploads/HJbNN1Wkgl.png)
- Dọc file và ta có mật khẩu: ```cat ./...Hiding-From-You```
- Mật khẩu: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
##Bandit4->5
- Đề bài: 
![image](https://hackmd.io/_uploads/H14oBy-yxx.png)
- Đề cho đoạn người đọc được -> dọc hết bằng lệnh ```cat ./*``` 
![image](https://hackmd.io/_uploads/rkmBIkWkxg.png)
- Mật khẩu: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
- À có thể kiểm tra file nào thuộc dạng đọc được bằng lệnh '''find . -type f | xargs file```
![image](https://hackmd.io/_uploads/ryKMu1Z1el.png)



