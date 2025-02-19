---
name: List environment secrets
example: octokit.rest.actions.listEnvironmentSecrets({ repository_id, environment_name })
route: GET /repositories/{repository_id}/environments/{environment_name}/secrets
scope: actions
type: API method
---

# List environment secrets

Lists all secrets available in an environment without revealing their
encrypted values.

You must authenticate using an access token with the `repo` scope to use this endpoint.
GitHub Apps must have the `secrets` repository permission to use this endpoint.
Authenticated users must have collaborator access to a repository to create, update, or read secrets.

```js
octokit.rest.actions.listEnvironmentSecrets({
  repository_id,
  environment_name,
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
    <tr><td>repository_id</td><td>yes</td><td>

The unique identifier of the repository.

</td></tr>
<tr><td>environment_name</td><td>yes</td><td>

The name of the environment.

</td></tr>
<tr><td>per_page</td><td>no</td><td>

The number of results per page (max 100).

</td></tr>
<tr><td>page</td><td>no</td><td>

Page number of the results to fetch.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/secrets#list-environment-secrets).
