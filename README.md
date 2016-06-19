# Notorious F.A.S.T.

High-speed, high-volume big data plumbing engine

Tribute to Notorious B.I.G.

## Concept code

Download source code in notfast-concept-code.zip to get idea of the architecture of Notorious Fast.

Working code may be added to a branch in this repository in a near future.

## Presentation

See the introduction slides in English and Japanese.

- notfast-intro-en.pdf
- notfast-intro-ja.pdf

## About

Notorious FAST (NotFast in short) is a generous purpose data receiver, notifier, organizer and saver designed to handle high-speed high-volume data.
It accepts data very fast and let an application display the data quickly.

Here is how it works:

- A queue is setup per data source.
- A queue handler thread reads data from a queue and spawns a worker thread.
- A piece of data can contain high priority and lower priority items.
- High priority items are immediately sent to display applications through UDP multicast.
- Lower priority items are saved to a data store for pickup by app when needed.

More contens will come soon.

Thank you.


