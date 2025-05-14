---
title: Eptura Visitor API Reference

language_tabs:
  - shell: cURL

toc_footers:
  - <a href='https://api.proxyclick.com/v1/docs'>Documentation Powered by Eptura Visitor</a>
  - <a href='https://www.proxyclick.com/api-access-request'>Request API access</a>

includes:
  - authentication
  - document
  - company
  - user
  - meeting
  - visit
  - visitor
  - custom_field
  - errors
  - webhooks
---

# Introduction

Welcome to the Eptura Visitor API! You can use it to access Eptura Visitor API endpoints.

You can view code examples in Shell in the dark area to the right.

# Summary

## Introduction

This part will explain shortly how the API needs to be consumed.

All API requests must be sent over HTTPS.
JSON is used in all responses : API data is JSON encoded with UTF-8.

The API also uses common approaches for the following

Function      | Description
------------- | -----------
Data          | API data is JSON encoded with UTF-8. API JSON is either a single object or a list of objects.
Authorization | Access control made by access token.
Errors        | 4xx and 5xx responses returning JSON with error codes, see [errors](#errors)
HTTP          | Methods are used in accordance with HTTP (GET, POST, PUT, DELETE and PATCH verbs are used but not for every URIs) and resources are identified using URIs. All API requests are sent over HTTPS.

&nbsp;

<aside class="notice">
All attributes in this documentation are considered as stable and backward compatibility will be provided. For this reason, we recommend to only use attributes that are publicly documented and ignore other attributes returned by the API.
</aside>

## Languages

The following language codes are accepted: `en` (English), `de` (German), `es` (Spanish), `fr` (French), `it` (Italian), `nl` (Dutch), `sk` (Slovak), `sl` (Slovenian), `vi` (Vietnamese), `ko` (Korean)

## Dates and timestamps

Dates and timestamps are ISO 8601 formatted (e.g. "2015-01-12T15:00:00+01:00").

See [Wikipedia](http://en.wikipedia.org/wiki/ISO_8601) for more information.

## Phone numbers

Phone numbers are E.164 formatted (e.g. "+12125551423").

See [Wikipedia](https://en.wikipedia.org/wiki/E.164) for more information.

Phone numbers are validated using the [libphonenumber](https://github.com/googlei18n/libphonenumber) library.
