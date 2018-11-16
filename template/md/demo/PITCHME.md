---
@title[demo - architect]

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
@title[demo - hardware]

@snap[north-west]
Phần cứng
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- DigitalOcean 5 * (2vCPU 4GB RAM) + 1 * (1vCPU 1GB RAM)
- domain: vuonghoaithu.name.vn 
- sadalmelik, sadalsuub, sadachbia, skat, albali, doitung
@ulend
@snapend

---
@title[demo - role]

@snap[north-west]
Vai trò
@snapend

@snap[west list-content-concise span-100]
@ul[](false)
- PostgreSQL: sadalmelik
- Hadoop: sadalmelik (namenode, worker); albali, doitung (worker)
- Zookeeper: sadalsuub, sadachbia, skat
- Druid: sadalsuub (overlord, coordinator), sadachbia (historical, middle manager), skat (broker)
@ulend
@snapend
