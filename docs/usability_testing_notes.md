# Usability Testing Notes

## Leanna S.

* Couldn’t find the "edit API" link

* Need "EDIT" header on edit link

* Need to change the hover on checkboxes on homepage

* Edit APIs is too broad.

* Need clearer instructions on GitHub

* Page did not change after save

* Maybe a color change?

* "Form did not submit"

* Save button would grey out because there are no new changes

* Would expect to see a blocker on red status APIs

* Need error message when things don’t save

* Multiple versions of APIs

## Rachel R.

**1. How would you determine the status of Benefits Intake API?**

* Important piece for scorecard like this.

* Each main API has a roadmap.

* There are multiple versions iterating on.

* Using this scorecard, assumed gathered requirements for each version, etc.

* Would need to cycle back through phases for a new version.

* For current APIs, not part of the beginning stages.

**2. How would you find a blocker for the test API?**

I would search for the test API and see block test.

**3. How would you change scorecard to change status of Benefits Intake API in order to raise a blocker?**

* Tried to change the status on the scorecard page.

* Don’t know how would change it on the Admin side.

* Was looking for a way to change status.

* Jumped down to status of the API.

* Clicked on GitHub link.

* Zoom screen was covering the Edit link

* Why we would need an OAuth token?

* Need to generate personal token.

* Created a token description.

* Doesn’t know which scopes to select.

* Didn’t generate the token with the repo selected.

* Going through process again.

* Clicked on Benefits Intake.

* What status to select that’s associated w/ a blocker?

* Typically blocker is data warehouse access or issue with stakeholders or last-min change in requirements.

* Change in requirements blocker and being in live stage doesn’t make sense.

* Why would there a be a blocker in the Live stage?

* Shouldn’t go live with potential blockers.

* After typing in the field, would press save.

* In 5 mins, going to redirect back?

* Or just assume need to wait in 5 mins?

* Clicked back.

**4. How to remove the blocker?**

* Go to edit APIs.

* Assuming can use the same token.

* If resolved, put back to green.

* Questioned what delete action would do?

* Changed to green and removed blocked reason.

* Wish was prompted to be able to in a comment about the status.

**5. Add an API to the scorecard.**

* Went to new API.

* Added new one.

* Looking for refresh of what different statuses mean.

* Looking for what statuses mean.

* Don’t know what grey means.

* Don’t know what to do with metrics.

* Going through the checklist in the Define stage.

* Unsure if she be checking off criteria in other stages.

**6. General thoughts.**

* Liked the interactive stages at top of scorecard

* When adding new API, would be helpful to have what color statuses mean (this wasn’t apparent at first)

* Liked the "sort by alphabet"

* Would like to be able to edit the API using a button/link associated with it from the scorecard page

* Need better description as to why an OAuth token is needed

* Couldn’t remember steps to generate a token

* Does homepage link field take you to the developer portal?

## Changes Made Based on Usability Testing

Summary of key changes we made based on the usability testing results:

* During testing, we observed that upon entering the admin panel, users would click on the GitHub link immediately without reading the instructions. They’d then typically create a token but gave it more permissions than necessary before returning to the site. As a result, we moved the GitHub link to the bottom of the instructions to nudge the user to at least skim the instructions before beginning the token creation process.

* The status control in the admin panel initially had just the status colors. After observing that users forgot the precise definitions of each status, we changed that status control to include the descriptions.

* We observed users being confused about changes being saved. We changed the state of buttons to indicate when changes had be saved or not.

* Observed confusion about whether a user was logged into the admin panel. Added logout and instruction changes based on if the user was logged in.

* Observed confusion when saved changes weren’t reflected on the form. Changed how forms were built to load immediately.
