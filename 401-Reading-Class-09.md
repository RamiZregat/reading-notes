# Authorization/Authentication

1. What header(s) are used in authentication and authorization?

- HTTP Basic Auth is a simple method that creates a username and password style authentication for HTTP requests. This technique uses a header called Authorization, with a base64 encoded representation of the username and password.

- In bearer authentication  HTTP authentication scheme that involves security tokens called bearer tokens. The name “Bearer authentication” can be understood as “give access to the bearer of this token.

2. What is safe to put into a JWT?

- JWS payload (set of claims): contains verifiable security statements, such as the identity of the user and the permissions they are allowed. JWS signature: used to validate that the token is trustworthy and has not been tampered with. When you use a JWT, you must check its signature before storing and using it.

3. How are JWTs validated?

- heck signature. The last segment of a JWT is the signature, which is used to verify that the token was signed by the sender and not altered in any way. The Signature is created using the Header and Payload segments, a signing algorithm, and a secret or public key (depending on the chosen signing algorithm).

## Vocabulary Terms

|      Word      |                                                      Definition                                                                                                  |
| :------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   RBAC   |  Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges                                                 |
|     User Roles    | User Roles are permission sets that control access to areas and features within the Professional Archive Platform.                                           |
|     JWT Token     | JSON Web Token (JWT) is a compact URL-safe means of representing claims to be transferred between two parties. |


## Preview

- Which 3 things had you heard about previously and now have better clarity on?
1. RBAC
2. ACL
3. Authentication in general

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
1. New things
2. AWS
3. Cleaner code

- What are you most excited about trying to implement or see how it works?
that the thing are really working with me smoothly as it working with the instructor.