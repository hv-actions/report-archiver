# Github action to archive a path into Practitest
## Using REST API
Example usage:
```
- name: Archiving Report
  uses: hv-actions/report-archiver@main
  with:
    lookup-folder: 'target/site/serenity'
    build-title: "Test Report for build ${{ github.run_number }}"
    project-id: <project_id>
    instance-id: <instance_id>
    practitest-api-host: https://eu1-prod-api.practitest.app
    practitest-host: https://eu1-prod.practitest.app
    practitest-token: ${{ secrets.PRACTITEST_PAT }}
```
