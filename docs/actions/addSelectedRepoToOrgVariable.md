---
name: Add selected repository to an organization variable
example: octokit.rest.actions.addSelectedRepoToOrgVariable({ org, name, repository_id })
route: PUT /orgs/{org}/actions/variables/{name}/repositories/{repository_id}
scope: actions
type: API method
---

# Add selected repository to an organization variable

Adds a repository to an organization variable that is available to selected repositories.
Organization variables that are available to selected repositories have their `visibility` field set to `selected`.

You must authenticate using an access token with the `admin:org` scope to use this endpoint.
If the repository is private, you must use an access token with the `repo` scope.
GitHub Apps must have the `organization_actions_variables:write` organization permission to use this endpoint.
Authenticated users must have collaborator access to a repository to create, update, or read variables.

```js
octokit.rest.actions.addSelectedRepoToOrgVariable({
  org,
  name,
  repository_id,
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
<tr><td>name</td><td>yes</td><td>

The name of the variable.

</td></tr>
<tr><td>repository_id</td><td>yes</td><td>

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/variables#add-selected-repository-to-an-organization-variable).
