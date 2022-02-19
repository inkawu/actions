# npm-version

## Usage
```yaml
- name: Version and push
  uses: inkawu/actions/npm-version@main
  with:
    commit_message: [The commit message of the push]
    name: [The name of the user that pushed the code]
    email: [The email of the user that pushed the code]
```

## Get commit variables
```yaml
env:
  commit_message: ${{ github.event.head_commit.message }}
  email: ${{ github.event.head_commit.author.email }}
  name: ${{ github.event.head_commit.author.name }}
```
