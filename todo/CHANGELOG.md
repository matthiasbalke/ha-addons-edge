- ci: use PAT for checkout to trigger CI via push event

Replace workflow_run trigger with PAT-based checkout so that
update-base-image pushes are treated as user actions, naturally
triggering CI via the existing push branch trigger.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>
