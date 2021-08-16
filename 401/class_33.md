## Review, Research, and Discussion

### Why is the Context API useful ? Context API is a way to enable components to share some data without explicitly passing via each component manually
### Can a component outside of a provider get its context ? No
### What are some common use cases for using the Context API ? Theming — Pass down app theme. i18n — Pass down translation messages. Authentication
### Describe “Context Hell” ? Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.


## Term
#### global state : a global state is a set of local states which are all concurrent with each other.
#### provider : makes the Redux store available to any nested components that need to access the Redux store.
#### consumer : A React component that subscribes to context changes.

## preperation material
### Role-Baed Access Control (RBAC):

#### As the name suggests, RBAC is a system that allow different access to users based on their roles.

####  EXAMPLES OF ACCESS CONTROL BASED ON ROLE Management role scope – it limits what objects the role group is allowed to manage. 

#### Primary – the primary contact for a specific account or role. Billing – access for one end-user to the billing account.

### react-cookie library
#### useCookies([dependencies])

#####Access and modify cookies using React hooks.

```const [cookies, setCookie, removeCookie] = useCookies(['cookie-name']);```
