# Robot Framework Request Action

This action runs Robot Framework tests using the [robotframework-request](https://github.com/Marketionist/robotframework-requests) library inside a Docker container.

## Example usage

```yaml
robot_test:
  runs-on: ubuntu-latest
  name: Run Robot Framework API Tests
  steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Run Robot Framework API Tests
      uses: yanaphatss/robotframework-request@v1.0.0
      with:
        test-path: "tests/"
```

## Inputs

| Input      | Description                             | Required | Default |
|------------|-----------------------------------------|----------|---------|
| test-path  | Folder or file containing test cases    | true     | -       |

## Outputs

_None_

## License

MIT
