---
name: Stop a codespace for the authenticated user
example: octokit.rest.codespaces.stopForAuthenticatedUser({ codespace_name })
route: POST /user/codespaces/{codespace_name}/stop
scope: codespaces
type: API method
---

# Stop a codespace for the authenticated user

Stops a user's codespace.

You must authenticate using an access token with the `codespace` scope to use this endpoint.

GitHub Apps must have write access to the `codespaces_lifecycle_admin` repository permission to use this endpoint.

```js
octokit.rest.codespaces.stopForAuthenticatedUser({
  codespace_name,
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
    <tr><td>codespace_name</td><td>yes</td><td>

The name of the codespace.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/codespaces/codespaces#stop-a-codespace-for-the-authenticated-user).
