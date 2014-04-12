# warrant

A **EXPERIMENTAL** golang implementation of the OpenStack Keystone(Identity) v3 JSON API

## What!? Why? Are you joking?

Serious. I have the need for an easy to run and deploy v3-like service that can
act as a drop-in replacement for the v3 API. Making that easy-to-deploy service
have no dependencies on virtualenv, pip and Python versions also sounds fun.

## What works?

This started as a need for a Keystone v3 proxy-like server that enabled local PKI
token validation without having to traverse a WAN. So, that's where I'm starting.

Assuming you have a valid token with the correct roles that allow you to validate
another Token you should be able to point that request at warrant and have it
exactly like a v3 request against Keystone.
