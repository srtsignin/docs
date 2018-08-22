# Overview

## Investment Themes

- Accurate Learning Center Usage Metrics

## Epics

- Student Sign-In
- Learning Center Reporting

## Features

- Student Classroom Sign-In
- Tutor Classroom Sign-In
<!-- - _Student In-Room Sign-In_ [^1]
- _Tutor In-Room Sign-In_ [^1] -->
- Learning Center Report Generation

## Stories

- As a student, I can sign in online to the percopo classroom so that I can receive help from a tutor.
    - LDAP username/password
    - ID Card
- As a student, I can submit feedback about my tutoring session to inform the learning center about my experience.
- As a tutor, I can check off when a student has completed their session so that the learning center knows about the session.

- As a learning center staff member, I can generate reports about classroom usage.
    - Total number of visits per week, quarter, year, etc.
    - Total number of visits per tutor.
    - Total session time per week, quarter, year, etc.
    - Total session time per tutor.
    - Total session time per student.
    - Students spending more than threshold (3 hours?)
    - Most frequent courses
    - Most frequent topics
    - Average student time spent per course
        - ex. MA courses might be 10 minutes, but CS courses might be 2 hours
    - Tutor ratings/comments

## Nonfunctional Requirements

- The system must authenticate users and provide authorized access to reporting information (NFR).

[^1]: _Items in italics are nice-to-have's._