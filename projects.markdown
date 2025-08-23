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
