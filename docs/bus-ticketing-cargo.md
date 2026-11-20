# 🚌 Bus ticketing & cargo platform

Software for intercity bus companies that sell seats and carry parcels on the same trips. Counter staff, drivers and station staff work on one shared system, and the owner sees the cash for every shift without adding anything up by hand.

**Live demo** (shared sample data, routes SG-CB / CB-SG, 28-seat buses):
- Online booking: [vexedemo.dulichreal.com](https://vexedemo.dulichreal.com/)
- Back office: [vexedemo.dulichreal.com/control2](https://vexedemo.dulichreal.com/control2), login `tester` / `tester`
- Step-by-step trial guide for bus operators (PDF, Vietnamese): [kich-ban-dung-thu-ve-xe-demo-cho-nha-xe.pdf](kich-ban-dung-thu-ve-xe-demo-cho-nha-xe.pdf)

## One working day on the system

```
Trips ──► Sell seats ──► Print lists for the driver
  │
  └──► Cargo: receive at office ──► load on trip ──► unload at station ──► deliver
                                                                              │
                                     End of shift: cash by trip and by staff ◄┘
```

## Trips

- Daily schedule is generated automatically, so every day already has trips to sell.
- Each trip holds the bus plate, bus type, driver and assistant with phone numbers, fare and notes.
- Add extra trips on busy days, or mark a trip as cargo-only.

## Seat tickets

| At the counter | Online (customer) |
| --- | --- |
| Seat map per trip; sell several seats in one go | Choose route, date and departure time (seats left and fare shown) |
| Caller recognised by phone number, with their other tickets that day | Pick seats on the seat map |
| Pick-up / drop-off points, shuttle fee, surcharge, discount; total calculated | Pick-up and drop-off points with a map |
| Payment: collected at office / by driver / not collected | Ticket code to open the ticket again |
| Move or swap seats, also to another trip; cancel one ticket or a whole group | If someone else just took the seat, the customer is asked to choose again |
| History of every ticket: who sold, changed or cancelled it, and when | |
| Print seat map, passenger list, pick-up list and shuttle list for the driver | |
| Search all tickets by the last digits of a phone number | |

Two counters selling the same trip never sell the same seat: the seat map refreshes every few seconds and double booking is blocked at the database level.

## Cargo

1. **Receive** at the office: sender, receiver, destination office (or roadside / door-to-door delivery), items, freight, COD; print a barcode label and an invoice.
2. **Load** the parcel on a trip.
3. **Unload** at the destination station.
4. **Deliver** to the receiver and collect what is still owed.

Each step can be done with the mouse from the station screens, or by scanning the label with a phone camera or barcode scanner. A parcel scanned at the wrong step is rejected with a low beep; a valid scan gives a high beep. Every parcel has a log of its whole journey, and staff always know whether it is at the sending office, on which bus, at the receiving station or delivered.

Station screens group parcels by state: newly received, on outgoing buses, on incoming buses, arrived, delivered, delivered by another office. Each list shows totals for freight paid by the sender, freight to collect on delivery, and COD.

## Cash control

- Ticket revenue by trip and route for any date range, with Excel export.
- Cargo cash per staff member per shift: freight collected when sending, freight collected on delivery, COD.
- One click turns a staff member's list into a collection receipt; receipts can be reviewed order by order.

## Built with

PHP · MySQL / MariaDB · JavaScript · runs on desktop browsers and phones (barcode scanning with the camera).

[← Back to profile](../README.md)
