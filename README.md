# Notorious F.A.S.T.

High-speed, high-volume data plumbing engine

Tribute to Notorious B.I.G.

## Concept code

Download source code in notfast-concept-code.zip to get idea of Notorious Fast architecture.

## Presentation

See the introduction slides in English and Japanese.

- notfast-intro-en.pdf
- notfast-intro-ja.pdf

## About

Notorious FAST (NotFast in short) is a generous purpose big data plumbing engine designed to handle high-speed and high-volume data.
It receives, notifies, organizes and saves data very fast and lets an application display the data quickly.

Here is how it works:

- A queue is set up per data source.
- A queue handler thread reads data from the queue and spawns a worker thread.
- A piece of data can contain high priority and lower priority items.
- High priority items are immediately sent to display applications through UDP multicast.
- Lower priority items are saved to a data store for pickup by app when needed.

More contents will come soon.

Thank you.


