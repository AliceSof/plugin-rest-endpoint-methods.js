---
name: Create or update a repository secret
example: octokit.rest.dependabot.createOrUpdateRepoSecret({ owner, repo, secret_name })
route: PUT /repos/{owner}/{repo}/dependabot/secrets/{secret_name}
scope: dependabot
type: API method
---

# Create or update a repository secret

Creates or updates a repository secret with an encrypted value. Encrypt your secret using
[LibSodium](https://libsodium.gitbook.io/doc/bindings_for_other_languages). For more information, see "[Encrypting secrets for the REST API](https://docs.github.com/rest/guides/encrypting-secrets-for-the-rest-api)."

You must authenticate using an access
token with the `repo` scope to use this endpoint. GitHub Apps must have the `dependabot_secrets` repository
permission to use this endpoint.

```js
octokit.rest.dependabot.createOrUpdateRepoSecret({
  owner,
  repo,
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
    <tr><td>owner</td><td>yes</td><td>

The account owner of the repository. The name is not case sensitive.

</td></tr>
<tr><td>repo</td><td>yes</td><td>

The name of the repository without the `.git` extension. The name is not case sensitive.

</td></tr>
<tr><td>secret_name</td><td>yes</td><td>

The name of the secret.

</td></tr>
<tr><td>encrypted_value</td><td>no</td><td>

Value for your secret, encrypted with [LibSodium](https://libsodium.gitbook.io/doc/bindings_for_other_languages) using the public key retrieved from the [Get a repository public key](https://docs.github.com/rest/dependabot/secrets#get-a-repository-public-key) endpoint.

</td></tr>
<tr><td>key_id</td><td>no</td><td>

ID of the key you used to encrypt the secret.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/dependabot/secrets#create-or-update-a-repository-secret).
