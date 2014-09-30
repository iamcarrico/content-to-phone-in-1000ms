## Results

* PageSpeed: 98
* YSlow: 98
* Pingdom: 93 w/ sub 500ms load time
* Web page test: 400-800ms load time (Usually As)

Note:
Some basic metrics put my site as incredibly fast (but please don't all go overload my servers!). YSlow and PageSpeed are both 98, and my two points I am missing are mostly out of my control. Doing some tests from Pingdom show that for the most part, content gets to the user under 500ms every time. Web page test puts my DOMContentLoaded at sub 500ms consistently, and the second page view is sub 250ms. I do get into trouble when users are very far away from one of my servers, or if DNS lookup takes too long. Even with those, I will still get consistantly under 1000ms for first page load.

http://tools.pingdom.com/fpt/#!/dhgR27/https://iamcarrico.com
http://tools.pingdom.com/fpt/#!/ca634J/https://iamcarrico.com
http://www.webpagetest.org/result/140930_T3_HMM/
http://www.webpagetest.org/result/140930_HW_HMR/
