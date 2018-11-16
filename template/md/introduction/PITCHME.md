---
@title[the-agenda]

@snap[north-west]
Mục lục
@snapend

@snap[west list-content-concise span-100]
@ol[list-bullets-black](false)
- Giới thiệu
- Kiến trúc hệ thống
- Truy vấn với Apache Druid
- Tích hợp với Apache Druid
- Demo
@olend
<br><br>
@snapend

--- 
@title[introduction1]

@snap[north-west]
Giới thiệu
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- Website: [druid.io](http://druid.io)
- Mã nguồn @fa[Github](https://github.com/apache/incubator-druid)
- Phần mềm nguồn mở, Apache License
@ulend
@snapend

---
@title[introduction2]

@snap[north-west]
Một vài cột mốc
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- Phát triển bởi [Metamarkets](https://metamarkets.com/) từ 2011
- Trở thành dự án nguồn mở vào cuối 2012
- Giấy phép
    + GPL
    + Apache V2 vào đầu năm 2015
- Được đóng góp bởi hơn 150+ lập trình viên
@ulend
@snapend

@snap[south-west template-note text-gray]
[scalable realtime analytics using druid](https://www.slideshare.net/HadoopSummit/scalable-realtime-analytics-using-druid)
@snapend

---
@title[motivation]

@snap[north-west]
Motivation
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- có rất nhiều các luồng sự kiện
    + call logs
    + network flows
- phân tích và tìm kiếm các thông tin có ý nghĩa
- giải pháp
    + hadoop: chậm
    + rdms, no sql architecture
@ulend
@snapend

@snap[south-west template-note text-gray]
[druid: a real-time analytical data store](http://static.druid.io/docs/druid.pdf) & [MetaMarkets - introduction to druid](https://www.youtube.com/watch?v=hgmxVPx4vVw)
@snapend

---
@title[usecases]

@snap[north-west]
Các công ty đang sử dụng Druid
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- [Danh sách](http://druid.io/druid-powered)
- [Netflix](http://techblog.netflix.com/2013/12/announcing-suro-backbone-of-netflixs.html)
- [Ebay](http://blog.csdn.net/ebay/article/details/50205611)
- [Cisco](http://www.networkworld.com/article/3086250/cisco-subnet/under-the-hood-of-cisco-s-tetration-analytics-platform.html)
@ulend
@snapend

@snap[south-west template-note text-gray]
[scalable realtime analytics using druid](https://www.slideshare.net/HadoopSummit/scalable-realtime-analytics-using-druid)
@snapend

---
@title[druid - a definition]

@snap[north-west]
một định nghĩa về druid
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- data store
- high-performance slice and dice analytics 
- large data sets
    - click stream analytics
    - network flow analytics
    - server metric storage
    - application performance metrics
    - digital marketing analytic
    - business intelligence / OLAP
@ulend
@snapend

--- 
@title[druid - key features]

@snap[north-west]
các chức năng nổi bật
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- columnar storage format
- scalble distributed system
- massively parallel processing
- self-healing, self-balancing, easy to operate
- cloud native, fault-tolerant architecture that won't lose data
- indexes for quick filtering
- approximate algorithms
- automatic summarization at ingest time
@ulend
@snapend

@snap[south-west template-note text-gray]
[druid: a real-time analytical data store](http://static.druid.io/docs/druid.pdf)
@snapend

