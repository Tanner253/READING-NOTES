# 5 steps to RBAC(ROLE BASED ACCESS CONTROL)

- what is RBAC?
  - RBAC is the action of assigning system access to an user based on their role in an organization (user vs admin).
  - Access is assigned to users based on their role assignment.
  - With the proper implementation of RBAC becomes systematic, and repeatable allowing easy ausdits of user rights.
  - Will prevent data breaches

1. Inventory your systems: Identify what resources you have, and who should be able to interact with them and in what ways.

2. Analyze workforce and create roles: Identiy what levels of access your application needs and who should have each type of access.

3. Assign people to roles.

4. Never make one off changes - THIS IS NOT A noSQL DATABASE, ALL MUST BE SAME (schema) change roles or add new ones when really necessary. 

5. Audit: Review roles database often to ensure proper access control.

I have used roles in recent applications in C#, They are a great way to secure the site.
RBAC is a new term for me but it makes sense and sounds nice.

#### Resources

[RBAC](https://www.youtube.com/watch?v=C4NP8Eon3cA)
[5 steps](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)