# UW-Madison-Course-Scraper
A Python script for scraping course data from (UW-Madison's course guide)[https://guide.wisc.edu/courses/].

Simply run,

```{Python}
course_scrape/fetch_all.py
```

and the script will scrape course info from `https://guide.wisc.edu/courses/` and will create a file `all-courses.json` within the parent directory that contains all course information for each course, including each course's:
  - Course Name
  - Course Subject
  - Course Code
  - Course Credits
  - Course Description
  - Course Prerequisites

An example of a course's information for UW-Madison's CS577 Introduction to Algorithms is as follows:
```{JSON}
"comp_sci 53": {
        "code": "COMP SCI 577",
        "name": "INTRODUCTION TO ALGORITHMS",
        "subject": "Computer Sciences",
        "credits": "4 credits",
        "description": "Basic paradigms for the design and analysis of efficient algorithms: greed, divide-and-conquer, dynamic programming, reductions, and the use of randomness. Computational intractability including typical NP-complete problems and ways to deal with them.",
        "requisite": "(MATH/COMPSCI240 or STAT/COMPSCI/MATH475) and (COMP SCI 367 or 400), or graduate/professional standing, or declared in the Capstone Certificate in Computer Sciences for Professionals",
        "last taught": "Last Taught: Fall 2022"
}
```
