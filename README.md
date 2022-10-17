# Github action to archive a path into Practitest

## Using firecracker CLI

Example usage:
```
- name: Archiving Report
  uses: hv-actions/report-archiver@firecracker
  with:
    lookup-folder: 'target/site/serenity'
    build-title: "Test Report for build ${{ github.run_number }}"
    project-id: <project_id>
    practitest-api-host: https://eu1-prod-api.practitest.app
    practitest-host: https://eu1-prod.practitest.app
    practitest-token: ${{ secrets.PRACTITEST_PAT }}
```
