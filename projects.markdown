---
layout: page
title: Projects
permalink: /projects/
---

This is the projects page. Here you will find select highlights of things I've hacked on.

## URL Shortener

Inspired by [this article](https://docs.shuttle.dev/templates/tutorials/url-shortener) on the [Shuttle](https://shuttle.dev) blog, I built my own, using Axum instead of Rocket.

A key difference in my version is integration testing. I worked out how to use the `testcontainers-modules` crate to mock a Postgres database for testing.

Code is here:

[Axum URL Shortener](https://github.com/crustyrustacean/url-shortener-v1)

## Pavex on Shuttle

[Shuttle](https://shuttle.dev) has been my platform of choice for building and deploying applications, ever since I discovered it in early 2023. The [Pavex](https://pavex.dev) web framework will likely become my go-to for developing APIs. I've been toying about with it since it made its debut in early 2024.

From the very day I discovered Pavex I asked the question, can it run on Shuttle?

The answer is a resounding yes. After much trial, error, and sweat, and also leaning heavily on [giants](https://blog.alexanderjophus.dev/posts/rust-full-stack-2/), it's possible:

[Pavex on Shuttle](https://github.com/crustyrustacean/pvx-on-shuttle)
