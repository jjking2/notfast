# Notorious F.A.S.T.

High-speed, high-volume big data plumbing engine

## Concept code

Download source code in notfast-concept-code.zip to get idea of the architecture of Notorious Fast.

Working code may be added to a branch in this repository in a near future.

## Presentation

See the introduction slides in English and Japanese.

- NotFastIntro-ja.pptx
- NotFastIntro-en.pptx

## About

Notorious FAST (NotFast in short) is a generous purpose data receiver, organizer and saver designed to handle high-speed high-volume data.
It accepts data very fast and let an application display the data quickly.

Here is how it works:

- A number of queues are set up to receive data.
- A queue handler thread reads data from one of the queues and spawn a worker thread.
- A piece of data can contain high-priority and normal-priority items.
- High-priority items are immediately sent to display applications through UDP multicast.
- Normal-priority items are saved to a data store.
- A display app reads the rest of data from the data storage when it needs it.

More contens will come soon.

Thank you.


