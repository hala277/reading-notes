# Authentication

## What is OAuth?

### 1. What is OAuth?

*OAuth is an open-standard authorization protocol or framework that explains how unconnected servers and services may properly enable authorized access to their assets without having to share a single login credential. This is referred to as secure, third-party, user-agent, delegated authorisation in authentication jargon.*

### 2. Give an example of what using OAuth would look like?

*is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.*

### 3. How does OAuth work? What are the steps that it takes to authenticate the user?

*Assume that a user has already joined up for a website or service (OAuth only works using HTTPS). The user then launches a feature/transaction that requires access to a separate site or service. The following occurs (oversimplified):*

1. *The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.*
2. *The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.*
3. *The first site gives this token and secret to the initiating user’s client software.*
4. *The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).*
5. *If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.*
6. *The user approves (or their software silently approves) a particular transaction type at the first website.*
7. *The user is given an approved access token (notice it’s no longer a request token).*
8. *The user gives the approved access token to the first website.*
9. *The first website gives the access token to the second website as proof of authentication on behalf of the user.*
10. *The second website lets the first website access their site on behalf of the user.*
11. *The user sees a successfully completed transaction occurring.*
12. *OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).*

### 4. What is OpenID?

*OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.*

-------------

## Authorization and Authentication flows

### 1. What is the difference between authorization and authentication?

*Authentication verifies that users are indeed who they claim to be. Authorization grants those users access to a resource.*

### 2. What is Authorization Code Flow?

*Regular web apps can utilize the Authorization Code Flow (specified in OAuth 2.0 RFC 6749, section 4.1), which trades an Authorization Code for a token, because they are server-side apps with no public source code. Because you must send along your application's Client Secret, which must always be kept safe, and you will have to keep it in your client throughout this exchange, your app must be server-side.*

### 3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

*The Authorization Code Flow may be used by mobile and native applications during authentication, however it requires additional protection. Furthermore, single-page apps have unique problems. To address these issues, OAuth 2.0 includes a Proof Key for Code Exchange version of the Authorization Code Flow (PKCE).*

### 4. What is Implicit Flow with Form Post?

*The Implicit Flow is an alternative to the Authorization Code Flow that is designed for Public Clients or applications that are unable to securely hold Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, it does provide a simplified workflow when combined with Form Post response mode if the application just requires an ID token for user authentication.*

### 5. What is Client Credentials Flow?

*Instead of a user, the system authenticates and authorizes machine-to-machine (M2M) applications such as CLIs, daemons, or services operating on your backend. Authentication techniques such as username + password or social logins are ineffective in this situation. M2M apps, on the other hand, employ the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4).*

### 6. What is Device Authorization Flow?

*Instead of immediately authenticating the user, input-constrained devices that connect to the internet ask the user to go to a URL on their computer or smartphone and approve the device. This prevents users from having a bad experience on devices that don't have a simple way to enter text. Device apps utilize the Device Authorization Flow to do this (drafted in OAuth 2.0). For usage with mobile and native apps.*

### 7. What is Resource Owner Password Flow?

*Highly-trusted apps can employ the Resource Owner Password Flow, which requires users to submit credentials (username and password) via an interactive form, however we do not encourage it. When redirect-based flows (such as the Authorization Code Flow) are unavailable, the Resource Owner Password Flow should be utilized.*

## Things I want to know more about

* *more about API*
