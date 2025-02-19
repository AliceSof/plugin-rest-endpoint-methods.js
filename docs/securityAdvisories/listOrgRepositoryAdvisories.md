---
name: List repository security advisories for an organization
example: octokit.rest.securityAdvisories.listOrgRepositoryAdvisories({ org })
route: GET /orgs/{org}/security-advisories
scope: securityAdvisories
type: API method
---

# List repository security advisories for an organization

Lists repository security advisories for an organization.

To use this endpoint, you must be an owner or security manager for the organization, and you must use an access token with the `repo` scope or `repository_advisories:write` permission.

```js
octokit.rest.securityAdvisories.listOrgRepositoryAdvisories({
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
<tr><td>direction</td><td>no</td><td>

The direction to sort the results by.

</td></tr>
<tr><td>sort</td><td>no</td><td>

The property to sort the results by.

</td></tr>
<tr><td>before</td><td>no</td><td>

A cursor, as given in the [Link header](https://docs.github.com/rest/guides/using-pagination-in-the-rest-api#using-link-headers). If specified, the query only searches for results before this cursor.

</td></tr>
<tr><td>after</td><td>no</td><td>

A cursor, as given in the [Link header](https://docs.github.com/rest/guides/using-pagination-in-the-rest-api#using-link-headers). If specified, the query only searches for results after this cursor.

</td></tr>
<tr><td>per_page</td><td>no</td><td>

The number of advisories to return per page.

</td></tr>
<tr><td>state</td><td>no</td><td>

Filter by the state of the repository advisories. Only advisories of this state will be returned.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/security-advisories/repository-advisories#list-repository-security-advisories-for-an-organization).
