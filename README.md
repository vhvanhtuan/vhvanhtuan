### Hi, I'm Tuan (Tony) Bui · Bùi Anh Tuấn

**Business Analyst & Senior Fullstack Developer** · Ho Chi Minh City, Vietnam

I turn how travel companies and bus operators actually run into software that runs every day: from business analysis and database design to coding and operations. I have led technical work and digitization at travel companies since 2005.

**What I build**

- Ticketing and cargo systems for bus operators: seat maps, double-booking prevented at the database level, 4-step cargo flow with QR scanning on phones, cash collection by office
- Travel company platforms: tour booking websites, group tours, visa, flights, hotels, car rental, CRM and back office
- Metadata-driven CMS back offices on React + PHP + MySQL

**Featured**

🌏 **Travel company platform** – one multi-tenant system that runs the websites and back office of travel companies. Sample sites (sample tour data): [site 1](https://vhv.dulichreal.com/) · [site 2](https://beta.dulichcongdongchaua.com/)

| Business line | What customers can do online | What staff manage in the back office |
| --- | --- | --- |
| Tours | Browse tours, departure calendar, book seats, look up a booking, pay | Tours, prices, departures, agents, suppliers |
| Group tours & gala events | Send a group request, receive a tailored proposal | Quotes, tour guides, services, payments |
| Car rental | Request a vehicle with driver | Contracts, vehicles, drivers, pricing |
| Bus tickets | Book seats on scheduled routes | Routes, trips, seat maps, tickets |
| Flights, hotels, visa | Send a booking or visa service request | Requests, bookings, status follow-up |
| Across all lines | | CRM, receipts and expenses, receivables, role-based permissions |

All modules run on the same metadata-driven CMS and auto-generated API, so each company's process can be adjusted without rewriting screens.

📄 Feature overviews (PDF, Vietnamese): [Travel platform](docs/dulichreal-platform-vi.pdf) · [Metadata-driven CMS](docs/cms-tu-sinh-vi.pdf) · live demo: [beta.dulichreal.com](https://beta.dulichreal.com/)

🚌 **Bus operator platform** – ticketing, cargo and cash control for intercity bus companies, used daily at the counter, on the bus and at every station. Live demo (shared sample data): [online booking](https://vexedemo.dulichreal.com/) · [back office](https://vexedemo.dulichreal.com/control2) (login `tester` / `tester`)

| Business line | What customers can do online | What staff manage in the back office |
| --- | --- | --- |
| Trips | See trips by route and date with seats left and fare | Daily schedule generated automatically; bus, driver and extra trips; cargo-only trips |
| Seat tickets | Pick a seat on the seat map, choose pick-up and drop-off points, get a ticket code | Sell several seats at once, move or swap seats (also to another trip), cancel; every change logged with who and when; print seat map, passenger and pick-up lists for the driver |
| Cargo | | Orders with COD, barcode label and invoice; load on a trip → unload at the station → deliver, by mouse or by scanning with a phone camera (a wrong step is rejected with a beep) |
| Cash control | | Ticket revenue by trip and route with Excel export; cargo cash collected by each staff member per shift; collection receipts |

Two counters selling the same trip never sell the same seat: the seat map refreshes every few seconds and double booking is blocked at the database level.

📄 [Full feature page: bus ticketing & cargo](docs/bus-ticketing-cargo.md) · [Trial guide for bus operators (PDF, Vietnamese)](docs/kich-ban-dung-thu-ve-xe-demo-cho-nha-xe.pdf)

**Stack**

React · JavaScript · PHP · MySQL · REST API · Docker · Claude Code

**How I work**

Interview the people who do the work → model the process and status flows → design the data → build → train staff → run and improve.

**Contact**

[LinkedIn](https://www.linkedin.com/in/tuan-bui-anh-70659784) · [thiendi.com](https://thiendi.com) · hb.anhtuan@gmail.com (Tuan / Tony)

---

<sub>Tiếng Việt: Phân tích nghiệp vụ và phát triển hệ thống quản lý cho công ty du lịch và nhà xe. Đang tìm vị trí BA / Senior Fullstack hoặc dự án triển khai trực tiếp.</sub>
