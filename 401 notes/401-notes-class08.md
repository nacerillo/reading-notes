# Class08 - Access Control

1. When is Basic Authorization used vs. Bearer Authorization?
   - Bearer Authorization is often recommended over using Basic as it offers more security. but Basic is easier, as it only requires a username and password, and does not require token generation
2. What does the JSON Web Token package do?
   - JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. [SOURCE](https://jwt.io/introduction) It is used for implement user authorization for a site. this is done by using a session ID. but instead of using cookies, it creates its own web token to do the authorization.
3. What considerations should we make when creating and storing a SECRET?
   - make sure that it is encrypted!

## VOCABULARY:

    - `encryption:` the scrambling and disguising of data, such as a users password or other person information, in order to hide it in a system.
    - `token:` it is a key that represents the user. it is used to identiy that the user is logged in, and does have access.
    - `bearer:`
    - `secret:` a secret code that is only known by the application that holds it. it protects an applications reoulses by only granting access to authorized users.
    - `JWT:`

## Preview:

    - Role Based Access Control: an approach to restricting system access to authroized users.
    - Five Steps to role-based access control:
        1. Inventory your systems:
        2. Analyize your workforce and create roles
        3. Assign people to roles
        4. Never make one-off changes
        5. Audit Aduit Aduit
