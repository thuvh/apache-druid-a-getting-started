---
@title[architect]

@snap[north-west]
Kiến trúc hệ thống
@snapend

@snap[midpoint span-90]
![Druid](template/img/druid-architecture.png)
@snapend

@snap[south-west template-note text-gray]
[druid: a real-time analytical data store](http://static.druid.io/docs/druid.pdf)
@snapend


---
@title[architect - middle manager]

@snap[north-west]
Middle Manager
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- đánh chỉ mục dữ liệu batch và realtime
- thông báo trạng thái và dữ liệu phục vụ cho zookeeper
- in-memory index buffer 
- persist to disk (đảm bảo bộ nhớ)
- sử dụng các block dữ liệu theo thời gian
- sẵn sàng phục vụ trong khoảng thời gian ngắn
@ulend
@snapend

---
@title[architect - historical]

@snap[north-west]
Historical
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- handle storage and query
- đóng vai trò chủ đạo trong hệ thống
- không thực hiện ghi dữ liệu (immutable object)
@ulend
@snapend

---
@title[architect - broker]

@snap[north-west]
Broker
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- giao diện của hệ thống đối với người dùng
- nhận các truy vấn và trả về kết quả
@ulend
@snape

---
@title[architect - coordinator]

@snap[north-west]
Coordinator
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- assign segment to specific server
- ensuring segments are well-balanced across Historicals
@ulend
@snape


