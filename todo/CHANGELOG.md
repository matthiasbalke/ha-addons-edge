- ci: trigger CI after update-base-image completes via workflow_run

Adds a workflow_run trigger so CI fires when the Update Base Image
workflow completes successfully on main. GitHub's GITHUB_TOKEN pushes
do not trigger downstream workflows, so this bridges that gap without
requiring a PAT.

Also fixes a misindented zizmor comment in deploy.yaml and removes
unnecessary quotes around `on` in update-base-image.yaml.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>
