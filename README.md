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

## Configure phases
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
## Configure statuses

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

## Configure edit form

The edit form can be reordered and new fields can be added by editing the `form_template.yaml` file.
1. Open `_data/form_template.yaml`
2. Make changes and commit the file to the `gh-pages` branch.
3. See file example below for description of fields.
```
- field_name: 'name' //must be unique, name of field
  type: 'text' //creates a text input field
  label: 'API Name'
  required: true
- field_name: 'description'
  type: 'textarea' //creates a text area field
  label: 'Description'
  required: true
- field_name: 'status'
  type: 'select' //creates a select box
  choices: 'statuses' //name of yaml configuration file
  label: 'Stage Status'
  required: true
- field_name: 'blocked'
  type: 'text'
  label: 'Status Description'
  required: true
- field_name: 'homepage'
  type: 'text'
  label: 'Homepage URL'
  required: false
- field_name: 'github'
  type: 'text'
  label: 'Github URL'
  required: false
- field_name: 'stage'
  type: 'select'
  choices: 'stages'
  label: 'Current Stage'
  required: true
- field_name: 'metrics'
  type: 'textarea'
  label: 'Metrics'
  required: false
- field_name: 'success_criteria'
  type: 'success-criteria' //Unique field type
  choices: 'stages'
  label: 'Success Criteria'
  required: true
```

## Running locally

1. Install `bundler`
  - `gem install bundler`
2. Run `bundle install`
3. Start server `jekyll serve`

## Some suggested improvements to the app

- Give it a proper datastore
- Rewrite using a backend framework such as Rails, which would make it less brittle, more generalizable (e.g., quickly build-out new scorecards), testable, etc.
- Integrate directly with GitHub repos to pull status
- Add admin form field validations
- Explore different ways of categorizing and visually communicating metrics
