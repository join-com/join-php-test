# Candidate Application & Score Calculator
![JOIN PHP Full-Stack Test](https://i.imgur.com/msT4Blg.png)

## Context

We love to give visual feedback to the recruiters about where their candidate stand in their pipeline.
Proposed solution consists of 2 screens:
1. *The applicant screen* - filling it in will send the application to the server
1. *The candidate list screen* - where all existing and new candidates can be viewed (reflecting input from the previous screen)

This app needs to display the list of candidates taken from this API: GET [https://join-candidates.free.beeceptor.com/api/candidate](https://join-candidates.free.beeceptor.com/api/candidate)
(If API is not available, use file located in this repository under /data/candidates.json) and send a local request instead.

## Design
Screens are provided in /data folder for reference, it doesn't have to look identical, just a visual reference, you can use Material or Bootstrap for UI components

## Requirements
As a Candidate:
- [ ] I want to be able to provide my data in application form without any field being required
- [ ] *[OPTIONAL]* I want to be able to upload my photo

As a Recruiter:
- [ ] I want to be able to view a list of my candidates
- [ ] For each application calculate score:
  - Up to 10% if full name provided
  - 10% if email provided
  - 10% if password provided
  - 20% if phone provided
  - *[OPTIONAL]* 50% if image uploaded (calculate accordingly if implemented or not)
- [ ] I want by clicking on the "..." menu, be able to "delete" the candidate (hide from display)
- [ ] I want by clicking on the "..." menu, be able to change candidate state from "submitted" to either "in review", "not a fit" or "hired"

## Technical Notes
- You can use Composer, npm or nothing, it's really up to you how to setup this application
- Please use PHP for this assignment, feel free to use pure language or any framework you like
- Use files or SQLite for storage
- Use either vanilla JavaScript or jQuery, you can of course go further and use anything else, but that's not necessary and gives no points
- If the external API is too slow, make sure it's not visible or felt by the user, find a way to make load/wait time a pleasure. Maybe kitten paws loader?
- You can download the existing candidates data into your database of choice (Files / SQLite / other) and make the application talk only with the database and not with the API endpoint we have provided
- *This test involves full-stack skills, you will have to put up a markup, style it with CSS, make async (AJAX) requests to the server, process it, store in DB and return a response to the client without a page refresh*

## Instructions
- Fork this repo
- Commit early and often. We want to be able to check your way of thinking
- Create a pull request so we can review your code and comment on it
- Do not spend more than 5 hours on the test, you will have a chance to submit fixes when our engineers review your code
- OPTIONAL: Make the app public. Deploy it using the service of your choice (Vercel, Cloud Run, Heroku)

## Disclaimer
You don't have to finish all of that, but we would really love to see a working piece.
What's more important for us is to see your way of thinking and priority on tasks during implementation!
