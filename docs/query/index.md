# Introduction

Patient Platform Query (PPQ) is a [graphql](https://graphql.org/learn) api implementation providing health information (the same information as served on https://patient.info)

The graph vocabulary is based on [Schema.org](https://schema.org) structured data but modelled for [PPQ](schema.md)

## Getting Started
In order to use PPQ you must have gained authentication credentials and authenticated using SSO with credentials that have access to the scope ```ppq:authenticated```, all requests to PPQ require an authentication header with a valid jwt ticket.