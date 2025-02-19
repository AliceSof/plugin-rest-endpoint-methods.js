---
name: Get a repository README
example: octokit.rest.repos.getReadme({ owner, repo })
route: GET /repos/{owner}/{repo}/readme
scope: repos
type: API method
---

# Get a repository README

Gets the preferred README for a repository.

READMEs support [custom media types](https://docs.github.com/rest/overview/media-types) for retrieving the raw content or rendered HTML.

```js
octokit.rest.repos.getReadme({
  owner,
  repo,
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
<tr><td>ref</td><td>no</td><td>

The name of the commit/branch/tag. Default: the repository’s default branch.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/repos/contents#get-a-repository-readme).
