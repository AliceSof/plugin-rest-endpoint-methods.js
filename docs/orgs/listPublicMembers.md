---
name: List public organization members
example: octokit.rest.orgs.listPublicMembers({ org })
route: GET /orgs/{org}/public_members
scope: orgs
type: API method
---

# List public organization members

Members of an organization can choose to have their membership publicized or not.

```js
octokit.rest.orgs.listPublicMembers({
  org,
});
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
    <tr><td>org</td><td>yes</td><td>

The organization name. The name is not case sensitive.

</td></tr>
<tr><td>per_page</td><td>no</td><td>

The number of results per page (max 100).

</td></tr>
<tr><td>page</td><td>no</td><td>

Page number of the results to fetch.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/orgs/members#list-public-organization-members).
