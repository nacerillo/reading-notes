# Class-07 Notes:

1. Order of steps in Requsting Token
   - Ask the client if they want to sign in via a third party
   - Make a request to a third-party API endpoint
   - Redirect to a third party authentication endpoint
   - Receive authorization code
   - Register your application to get a client_id and client_secret
   - Make a request to the access token endpoint
   - Receive access token
2. What can you do with access tokens?
   - Allows you to make request to APIs on behalf of the user. The token can also give authorization of to a specific application to access specific parts of a user's data. Access tokens must be protected at all times!
3. Benefits of OAuth
   - OAuth allows for access to other kinds of user data without compromising the users security credentials.

## Vocabulary:

- **ClientID:** An public identifier for an application
- **Client Secret:** An identifier/code that is only known to your application and it's server. it is used to grant access tokens only to authorized users.
- **Authentication Endpoint:** use by a device to gain access to a specifc webaite or network. Ensures that only specific devices can enter [SOURCE](https://www.techopedia.com/definition/23918/endpoint-authentication)
- **Access Token Endpoint:** used to request for a new access token on refresh.
- **API Endpoint:** used to open communication and passing of information bewteen two system or programs. Each time we want to access data from an api, we have to use the proper URI.
- **Authorization Code:** A password that is used to enter information into a protected space. usually associated with OAuth.
- **Access Token:** a token that is used for authentication, which allows an application to access an API. [SOURCE](https://auth0.com/docs/tokens/access-tokens)
