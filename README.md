# VA API Scorecard

A dashboard for tracking the status and phases of development for APIs at the VA.

## Setup

1. Fork the repo
2. On the new repo visit github `Settings` tab.
  - Ensure gh-pages is enabled
  - Ensure branch is set to gh-pages
3. Edit `_config.yml` file.
4. Change `github_user` to the user name of the repo owner
5. Change `gihub_repo` to the repo name
6. **Note:** In order for users to edit API statuses using the edit page, they must have read and write access to this repo.

## Configure Phases
Phases can be configured and will be reflected automatically after the site rebuilds on github pages. 

**Note: Changes to phases will not update phases of APIs. They will need to be updated seperately**

To change phase names and steps
1. Open `_data/stages.yaml`
2. Make changes and commit the file to the `gh-pages` branch.
3. See file example below for description of fields.
```
- name: Define // Name of the stage
  steps: // Success Criteria Steps. Index controls order, must start with 0.
    - text: Product vision is defined and aligns to a strategic imperative
      index: 0
    - text: Identified and documented who the primary users are and what their needs are through primary research
      index: 1
 ```
## Configure Statuses

Statuses can be configured and will be reflected automatically after the site rebuilds on github pages. 
1. Open `_data/statuses.yaml`
2. Make changes and commit the file to the `gh-pages` branch.
3. See file example below for description of fields.
```
- name: 'Grey' //Name stored in the API config files
  image: 'assets/img/alerts/grey-circle.svg' //Path to the status icon
  alt: 'Not yet started' //Text used for alt tags and edit form
- name: 'Yellow'
  image: 'assets/img/alerts/yellow-circle.svg'
  alt: "Having issues, but we're managing"
- name: 'Green'
  image: 'assets/img/alerts/green-circle.svg'
  alt: 'Overall things are going well'
- name: 'Red'
  image: 'assets/img/alerts/red-circle.svg'
  alt: 'Experiencing major blockers to success'

```

## Running locally

1. Install `bundler`
  - `gem install bundler`
2. Run `bundle install`
3. Start server `jekyll serve`
