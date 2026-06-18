# US History 8 Course Dashboard

Static reviewer dashboard generated from the Canvas course planning project.

Open the dashboard:

https://bbuchler.github.io/us-history-8-2-course-dashboard/

## Update workflow

From `C:\school\canvas-course-creation`:

```powershell
$env:Path = "$env:USERPROFILE\node-portable\node-v24.13.1-win-x64;$env:Path"
node scripts/update-build-tracker.js 8-2 3769
node scripts/export-outline.js 8-2
node scripts/export-static-dashboard.js 8-2
```

Then push the contents of `course_planning/reviewer-dashboard` to this repository.

No Canvas API token, Firecrawl key, or local .env file is included.
