---
name: Get a blob
example: octokit.rest.git.getBlob({ owner, repo, file_sha })
route: GET /repos/{owner}/{repo}/git/blobs/{file_sha}
scope: git
type: API method
---

# Get a blob

The `content` in the response will always be Base64 encoded.

_Note_: This API supports blobs up to 100 megabytes in size.

```js
octokit.rest.git.getBlob({
  owner,
  repo,
  file_sha,
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
<tr><td>file_sha</td><td>yes</td><td>

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/git/blobs#get-a-blob).
