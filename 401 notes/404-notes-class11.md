# Class 11 Notes: Event Driven Applications

1. Why is access control important
   - for some applications, it is prudent that access to some features and information be restricted to only a small number of users. or none at all
   - It protects important user data, and prevents some users from tamering with sensitive elements of an application
2. Describe an application that would need access control.
   - any site that relies on logging in users. users need to have their credentials that are protected, and that allow them to access what they need, and only what they need.
   - Sites that require admins to manage them and their users.
3. What is a role used for
   - A role defines what actions a user can take on a cite, and determines their level of access.
4. Why is role based access control more scalable than discretionary or mandatory access control?

- [SOURE](https://www.techotopia.com/index.php/Mandatory,_Discretionary,_Role_and_Rule_Based_Access_Control)

  - `Mandatory Access Control:` Enforced environment access to all resource objects - such as data files - is controlled by settings defined by the system administrator.
  - `Discresionary Access Control:` Allows each user to control access to their own data. DAC is typically the default access control mechanism for most desktop operating systems.
  - Roled Based Access Control is more scalable than these approaches b/c it allows for a more diverse range of use-cases for different users....

  ## Vocab:

  - `Authorization:` a secrutiy method to determine access levels or user capabilites related to an application.
  - `Capabilites: ` refers to the type of actions such as _delete, update, create and read_ that a user can take on a site based on their Authorization.
  - `Role Based Access Control`: users are assigned roles, and these roles determine what capabilites they have.
