# Run private composite action

This is a GitHub Action to run private composite actions. 


## Usage

```
  - name: Fetch private action
    uses: jusbrasil/run-private-action@main
    with:
      repo: {org}/{repo}
      token: ${{ secrets.GITHUB_TOKEN }}
      actionPath: node/setup
```

## Options

The following input variables options must be configured:

|Input|Description|
|----|----|
|`repo`|The private repo with the action that will be cloned|
|`token`|Your github token to access the private repo|
|`actionPath`|Which action to execute|
