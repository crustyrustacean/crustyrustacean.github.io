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

## Pavex and Tera Templates

Pavex is still in active development, so it's missing still a few essentials. I built a library which leverages the `tera` crate for HTML templating.

[FLux HTML Template](https://github.com/crustyrustacean/flux_html_template)

Just to be clear, this library is in no way affiliated with the main Pavex project.

## Pavex and Static Files

Pavex also lacks a means of serving static assets, such as CSS and JavaScript. I built a library to achieve this.

[Flux Static Files](https://github.com/crustyrustacean/flux_static_files)

## Axum Template (for Shuttle)

I've built an opinionated starting template for Axum API projects. Using [Cargo Generate](https://cargo-generate.github.io/cargo-generate/index.html) you can use my template to rapidly spin up a starting point and embelish it with your own API logic.

Code is here:

[Shuttle Template Axum](https://github.com/crustyrustacean/shuttle-template-axum)

I also built a variation of this template adds HTML templating with [Tera](https://keats.github.io/tera/) and static asset serving via `ServeDir` from [tower-http](https://crates.io/crates/tower-http). Static assets such as CSS, images, and JavaScript can be served up.

Code is here:

[Shuttle Template Axum Tera](https://github.com/crustyrustacean/shuttle-template-axum-tera)

## Fun with Nom

In late 2023 and early 2024, I developed an odd obsession with the [nom](https://crates.io/crates/nom) crate. I built an API which, in theory, might turn into something to count words. Dusted it off and updated it with my Axum API template. Also meant it to be a jumping off point for those learning with Nom, as many of the resources I found were quite outdated.

Code is here:

[Fun with Nom](https://github.com/crustyrustacean/fun-with-nom)

## Hyper-Actor Template (for Shuttle)

In the spring, my Rust instructor from ZTM inspired me to have a look at actors. They may be a poor architectural choice for Rust, but it was educational to work through some concepts, including some basic Rust concurrency building blocks. I built a frankenstein thing leveraging the `hyper` crate. It's a basis for a simple web API, with some rudimentary starting actors, that could be the basis of something bigger. I have this sort of silly dream of making something that's automated that can run tasks and otherwise do my bidding. This might be the basis...someday.

Code is here:

[Shuttle Template Hyper Actor](https://github.com/crustyrustacean/shuttle-template-hyper-actor)
