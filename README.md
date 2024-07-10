# TheForum API for Moderators

This repository contains the OpenAPI specification for the `TheForum` API for moderators. This API allows forum moderators to manage posts and users on the forum.

## Overview

- **API Version:** v1
- **Base URL:** `https://theforum.com/api/v1/moderator`
- **Authorization:** Bearer Token (JWT)

## Getting Started

### Prerequisites

- [Swagger editor available locally](https://swagger.io/tools/swagger-editor/download/) / a cloud [Swagger Editor](https://editor-next.swagger.io/) /any other OpenAPI-compatible tool of your choice
- Bearer Token for authorization (could be retrieved in your forum profile)

### Usage

1. **Clone the Repository:**

   ```sh
   git clone https://github.com/maximkuzmin/forum_moderators_api_doc.git
   cd forum_moderators_api_doc

2. Open the OpenAPI Specification:

    Open the openapi.yaml file in Swagger Editor or any other OpenAPI-compatible tool to explore and interact with the API.


### Notes on extension of an API
1. Please, use usual REST design best practices
    - use nouns for resources, not verbs
    - use existing naming convention in `snake_case` for resource and parameter names
    - use same PaginatedResponse object for each index resource that could have list of results which are more than 5
    - use same page and and page_size parameters in  such paginated resources
    - use suitable REST methods for the actions, don't index with POST and get data with DELETE

### TODO
There are definitely ways to improve a spec for an API, like this:
1. Specify rate-limits of the API
2. Specify error codes for each endpoints (404s, validations errors, etc)
3. Improve information about security
4. Add endpoints for token issuing and exchanging

