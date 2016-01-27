# SDLC
## Inception
Each line item forms the basis for the next
- Obtain requirements (can be high level, include time constraints)
  - Create `repository`
  - Create `README.md`
- Draft initial scope
  - Update `README.md`
- Develop design and team review it (can be multiple sessions)
  - Create `doc/DESIGN.md` or could be in `Wiki` 
  - Iteratively revised during *construction*
- Generate tasks (can include tasking to Ops/Plans)
  - Create `issues`
- Create an initial release plan. May take multiple (internal) releases to reach a deployable release. Each internal release should be a working release with subset of features
  - Create `milestones` and group `issues`
  - Set `assignees`
  - Set `milestone expiry dates`

## Construction
- Always create feature branches to avoid contaminating `master`
- Submit a merge request so that owner can merge commits into protected master
- Peer review merge request using comments
- Develop code to close `issues` and achieve `milestone`
  - Reference issue in commit message to auto-close issue
  - See [COMMIT](COMMIT.md) for commit guidelines
- Demonstrate `milestone` release to seek feedback. This goes into updating all the initial drafts during *inception*. May also result in new features to be added as `issues`
- Repeat for next milestone until fit for transition

## Transition
- Acceptance testing
- Create release `branch`
  - Cherry picking of critical bug fixes into stable release `branch`
  - New features go into master branch
  - See https://about.gitlab.com/2014/09/29/gitlab-flow/
- Trial

## Production
- Bug reporting and fixes
  - Need reporting system? Register bugs as `issues`


