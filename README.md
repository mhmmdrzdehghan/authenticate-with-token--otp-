# One-Time Password (OTP) Login System – Laravel API

This project demonstrates a *token-based login system using One-Time Passwords (OTP). It is developed using **Laravel 12* and is *fully API-based. Users can log in using a 6-digit OTP sent to their email. Authentication is handled via **Laravel Sanctum*.

> *Only core and essential files* are included in this repository for *code review* purposes.  
> *This project is for portfolio demonstration only and is not intended to be used as a package or production-ready code.*

---

## Features

- *OTP Generation & Email Sending*
  - A 6-digit random code is generated and sent on every login request
  - The code expires after *1 minute*
  - Emails are dispatched using Laravel's *Queue & Job* system
  - The queue driver is set to database for faster email delivery

- *OTP Login*
  - Users log in by submitting the received OTP
  - Secure token-based authentication using *Laravel Sanctum*

---

## Tech Stack

- Laravel 12
- Laravel Sanctum
- MySQL
- Laravel Queues & Jobs (with database driver)
- Mail Configuration (email-based OTP delivery)

---

## Architecture

- The entire system is *API-driven*, designed to be consumed by frontend clients or mobile applications.
