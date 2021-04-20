# Shortening the size of the URL
>@cleisonmelo

[![Angular](https://img.shields.io/badge/Angular-11.0-DD0031.svg)](https://angular.io/)
[![Golang](https://img.shields.io/badge/Golang-1.16-00ACD7.svg)](https://golang.org/)
[![Redis](https://img.shields.io/badge/Redis-6.2-A41F16.svg)](https://redis.io/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4.4-10AA50.svg)](https://www.mongodb.com/)
[![Docker](https://img.shields.io/badge/Docker-2.3-2496ED.svg)](https://www.docker.com/get-started)
___

  > URL shortening is used to create shorter aliases for long URLs. We call these shortened aliases “short links.” Users are redirected to the original URL when they hit these short   links. Short links save a lot of space when displayed, printed, messaged, or tweeted. Additionally, users are less likely to mistype shorter URLs.

## Functional Requirements

* Given a URL, our service should generate a shorter and unique alias of it. This is called a short link. This link should be short enough to be easily copied and pasted into applications.
* When users access a short link, our service should redirect them to the original link.
* Users should optionally be able to pick a custom short link for their URL.
* Links will expire after a standard default timespan. Users should be able to specify the expiration time.

## Non-Functional Requirements

* The system should be highly available. This is required because, if our service is down, all the URL redirections will start failing.
* URL redirection should happen in real-time with minimal latency.
* Shortened links should not be guessable (not predictable).

## Extended Requirements

* Analytics; e.g., how many times a redirection happened?
* Our service should also be accessible through REST APIs by other services.
