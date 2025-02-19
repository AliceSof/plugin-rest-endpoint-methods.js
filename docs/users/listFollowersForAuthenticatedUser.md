---
name: List followers of the authenticated user
example: octokit.rest.users.listFollowersForAuthenticatedUser()
route: GET /user/followers
scope: users
type: API method
---

# List followers of the authenticated user

Lists the people following the authenticated user.

```js
octokit.rest.users.listFollowersForAuthenticatedUser();
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>per_page</td><td>no</td><td>

The number of results per page (max 100).

</td></tr>
<tr><td>page</td><td>no</td><td>

Page number of the results to fetch.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/users/followers#list-followers-of-the-authenticated-user).
