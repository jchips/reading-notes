# Reading Notes 8

This topic is important for implementing authorization into a project.

## 5 steps to RBAC

What is Role Based Access Control (RBAC) and why do we care?

- "Role-Based Access Control (RBAC) is a security paradigm that restricts system access to authorized users based on their roles and responsibilities within an organization. In RBAC, permissions are associated with roles, and users are assigned to specific roles based on their job functions. This approach helps organizations manage and control access more effectively than assigning permissions directly to individual users." - ChatGPT. We care because then we can make sure only authorized users get access to certain parts of our software that we want to limit eyes on, so we care about it because of security.

Describe a Role/Permission heirarchy that you might implement using RBAC.

- Base level: maybe **guests** have permission to read data.
- 2nd level: a **user** that can read and write data to their own profile and read public stuff.
- 3rd level: a moderator has all the permissions the user has, can read and write access to user-generated content and can **moderate** and delete comments or posts.
- Highest level: An **admin** has all permissions that the moderators do. They also have full control over user management (create, modify, delete users), full control over content management (create, modify, delete any content), and access to system configuration settings.

What approach might you take to implement RBAC?

- First, identifying the different roles and permissions. Then adding them to the table model. Then implementing the access control so that only people with certain roles can access what they have permission to. Then create tests and make sure they all pass.

Source: ChatGPT

## wiki - RBAC

If Authentication is “you are who you say you are,” what is Authorization?

- If you are who you say you are, you can access this information. If not, then you can't.

Name three primary rules defined for RBAC.

- "Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role." - Wikipedia
- "Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized." - Wikipedia
- "Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized." - Wikipedia

Describe RBAC to a non-technical friend.

- RBAC aka role-based access control is when different roles can access different stuff or have permissions to do different things. For example, if you are a guest, you may only have permission to read information from something, but if you are an admin, you have permissions to read and write and access information that guests aren't allowed to. So, implementing RBAC is giving different people on a hiearchy different permissions and access.

Source: <https://en.wikipedia.org/wiki/Role-based_access_control>

## RBAC tutorial

What are access rights associated with? The User? or The Role? Explain.

- Access rights are associated with the role. So, for each role, question what kind of resources do they need to have access to? Those become the access rights. The role is associated with the user I think.

Access Rights, or Authorization, is activated after a user successfully does what?

- Successfully is authenticated.

Explain how RBAC might benefit a business.

- As soon as a new employess comes in, their role is decided. So, policies don't have to be changed when new people come and go. They just get assigned a role and then have rights and permissions limited to that role.

Source: <https://www.youtube.com/watch?v=C4NP8Eon3cA>

## Reflection

My learning goals are learning/understanding how to implement RBAC into a project.

## Things I want to know more about
