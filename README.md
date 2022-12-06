# Metro Transit NexTrip API Definition 🚍

This provides an [OpenAPI](https://github.com/OAI/OpenAPI-Specification) definition for the [Metro Transit NexTrip API](https://svc.metrotransit.org/swagger).

## ReadMe Documentation :owl:

[The OpenAPI file in this repository](./openapi.json) backfills [the server object](https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#serverObject) so the API can be used in [these unofficial docs](https://metrotransit.readme.io/reference), hosted on [ReadMe](https://readme.com/). The file is syncing to ReadMe via a [GitHub Action](https://github.com/readmeio/rdme).

## Update (December 2022)

Metro Transit released version 2[^1] of [the NexTrip API](https://svc.metrotransit.org/swagger), along with [an entire OpenAPI definition](https://svc.metrotransit.org/swagger/docs/v2/nextrip) to boot! See a screenshot of the deprecation notice below (grabbed from [here](https://web.archive.org/web/20221111210238/https://svc.metrotransit.org/)):

<img width="791" alt="A screenshot of a deprecation notice that reads: 'NOTICE: NexTrip version 1 (https://svc.metrotransit.org/nextrip/) is deprecated and will be removed at the end of June '22.
Version 2 documentation can be found at https://svc.metrotransit.org/swagger.'" src="https://user-images.githubusercontent.com/8854718/205979280-a8ee7a8e-5f17-4fab-9d9f-0b71680aace8.png">

This repository was created a few years ago to document version 1 of the API, back when it was primarily returning XML responses and the only official documentation was [a static, non-interactive page with a list of endpoints](https://web.archive.org/web/20220319192455/https://svc.metrotransit.org/NexTrip). How far we've come 🥹

While this is all very exciting news, this repository is no longer a good source-of-truth for the NexTrip API and you should refer to [the official docs](https://svc.metrotransit.org/swagger) instead.

If you're looking for an official demo of [the `rdme` GitHub Action](https://github.com/readmeio/rdme), please check out [this repository](https://github.com/readmeio/rdme-demo).

[^1]: As of this writing (12/6/2022), the docs say that the API is still in beta and is subject to change.
