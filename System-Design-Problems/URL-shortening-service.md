## 1. Why do we need URL shortening

It can shorten the URL and save a lot of space.

## 2. Requirements and goals of the system

The URL shortening system should meet the following requirements.

- Functional Requirements
  - Given a URL, our system would generate shorten URL.
  - The short link would direct user to the orginal URL page.
  - Users could optionally be able to pick a custom short link for the URL.
  - Links would be expired by the set time span. There is a default time span and users can also define it.
- Non-Functional Requirements
  - The service should be highly avaliable.
  - URL direction should be real-time with minimun latency.
  - Short link is not predictable.
- Extended Requirements
  - Analytics
  - The service should be accessible through REST APIs by other service.