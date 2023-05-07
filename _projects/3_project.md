---
layout: page
title: Multi-Threaded, Caching TCP Proxy Server
description: Assignment for Network Systems
img: assets/img/proxy_serv.png
importance: 3
category: work
---

This project represents the the most complex and challenging software that I have ever written. All told, I estimate that I spent upwards of 60 hours on this assignment. The program is written in C, and it is a working multi-threaded proxy server capable of caching and serving recent web pages, and is able to service multiple clients in parallel. 

The concurrency considerations made this program particularly challenging to implement, as the server must not only communicate with multiple clients in parallel, but must also cache webpages in a thread-safe data structure. In this case, that data structure is a hash-table that handles collisions via chaining with linked lists. Each list is protected by a special reader / writer semaphore from the POSIX pthreads library, which allows multiple readers to access its contents at any given time, but locks down the linked list if any writers are present. This implementation limits the size of critical sections of code and allows for a high degree of parallelism. 

A project like this is never really complete - commercial proxy servers are generally millions of lines of code, account for an incredible number of contingencies and idiosyncrasies, and require constant maintenance to operate effectively in the dynamic and ever-changing environment that is the modern internet. Nevertheless, this program does work, and I'm proud to have written it. 