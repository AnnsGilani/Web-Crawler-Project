# Multithreaded Web Crawler (C++)

This project is a multithreaded web crawler implemented in C++ using POSIX threads
and libcurl. It demonstrates core Operating System concepts such as multithreading,
synchronization, and the producer–consumer problem.

---

## Features
- Multithreaded crawling using pthreads
- Thread-safe URL queue (producer–consumer model)
- Domain restriction
- Depth limiting
- Maximum pages limit
- HTML parsing using regex
- Saving downloaded pages locally
- Logging and crawler statistics

---

## Technologies Used
- C++ (C++11)
- POSIX Threads (pthreads)
- libcurl
- Linux (Ubuntu / WSL)

---

## How to Run

```bash
g++ crawler.cpp url_queue.cpp parser.cpp stats.cpp logger.cpp saver.cpp -o crawler -lpthread -lcurl
./crawler https://books.toscrape.com
