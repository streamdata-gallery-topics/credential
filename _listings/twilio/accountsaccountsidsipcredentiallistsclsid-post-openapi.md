---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Add SIP Credentials List
  description: Change the FriendlyName of the list
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/CredentialLists:
    get:
      summary: Get SIP Credentials List
      description: Gets a list of Credential Lists for an account
      operationId: gets-a-list-of-credential-lists-for-an-account
      x-api-path-slug: accountsaccountsidsipcredentiallists-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
    post:
      summary: Get SIP Credentials List
      description: Create a new Credential List.
      operationId: create-a-new-credential-list
      x-api-path-slug: accountsaccountsidsipcredentiallists-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
  /Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}:
    delete:
      summary: Delete SIP Credential List
      description: Delete a CredentialList from your account. It can only be deleted
        if no domains are mapped to it. If you attempt to delete one that is mapped
        to a domain, you will receive an error.
      operationId: delete-a-credentiallist-from-your-account-it-can-only-be-deleted-if-no-domains-are-mapped-to-it-if-y
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
    get:
      summary: Get SIP Credentials List
      description: Get a credential list instance resource
      operationId: get-a-credential-list-instance-resource
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
    post:
      summary: Add SIP Credentials List
      description: Change the FriendlyName of the list
      operationId: change-the-friendlyname-of-the-list
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---