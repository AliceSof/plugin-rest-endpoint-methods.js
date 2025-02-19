---
name: Get an organization secret
example: octokit.rest.actions.getOrgSecret({ org, secret_name })
route: GET /orgs/{org}/actions/secrets/{secret_name}
scope: actions
type: API method
---

# Get an organization secret

Gets a single organization secret without revealing its encrypted value.

You must authenticate using an access token with the `admin:org` scope to use this endpoint.
If the repository is private, you must use an access token with the `repo` scope.
GitHub Apps must have the `secrets` organization permission to use this endpoint.
Authenticated users must have collaborator access to a repository to create, update, or read secrets.

```js
octokit.rest.actions.getOrgSecret({
  org,
  secret_name,
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
<tr><td>secret_name</td><td>yes</td><td>

The name of the secret.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/secrets#get-an-organization-secret).
