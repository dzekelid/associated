swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/associated:
    get:
      summary: My Assocated
      description: "Returns all of a user's associated accounts, given an access_token
        for them.\n \nThis method returns a list of network users."
      operationId: returns-all-of-a-users-associated-accounts-given-an-access-token-for-them-this-method-returns-a-list
      x-api-path-slug: meassociated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Associated
  /users/{ids}/associated:
    get:
      summary: Get User Associated
      description: "Returns all of a user's associated accounts, given their account_ids
        in {ids}.\n \n{ids} can contain up to 100 semicolon delimited ids, to find
        ids programatically look for account_id on user objects.\n \nThis method returns
        a list of network_users."
      operationId: returns-all-of-a-users-associated-accounts-given-their-account-ids-in-ids-ids-can-contain-up-to-100-
      x-api-path-slug: usersidsassociated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Users
      - Associated