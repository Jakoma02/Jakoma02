# GSoC 2025 Final Work Submission

- Organization: [Learning Equality](https://learningequality.org/)
- Project: Kolibri Community Library
- Mentors: Richard Tibbles and Alex Velez

## Project Goal

The goal of the project was to add a Community Library feature to the Kolibri ecosystem. This feature would allow content creators to submit their channels
to the Community Library. After approval of the submission by the organization administrators, users would be able
to import the channel from the Community Library into Kolibri.

## Accomplished Goals

The backend API of the Kolibri Studio content curation platform was extended with most functionality needed to support
the operation of the Community Library. This included the support for creating Community Library submissions
and listing them, and approving/rejecting submissions by organization admins. Many changes needed to be made to 
support these features and to ensure their correct behavior in the production Kolibri Studio environment.

The Kolibri Studio frontend was updated with several key features to allow integration of the Community Library functionalities.
An interface that allows administrators to list and filter channels on the platform was extended to allow displaying and filtering
by the Community Library submission status of the channel.
This required extensive changes to the filtering system used in the project codebase. An interface for content creators
was also added to allow submitting a channel to the Community Library.

All newly created code included automated tests to provide confidence in the provided changes, and the code
tried to adhere to best practices and high coding standards.
Please see the [Pull Requests](#pull-requests) section for more details about the specific changes implemented during the project.

## Current State

The backend part of Kolibri Studio is mostly ready to support the Community Library feature in the Studio platform, and is
reasonably prepared for an interface for interaction with Kolibri to be implemented.

Several key features have been implemented in the frontend part of Kolibri Studio, but a large portion of the user experience
is currently missing. It is possible to submit channels to the Community Library via the web interface, and admins can see
channels together with their submission status. On the other hand, as of now, the functionality to review submissions to the
Community Library or browsing channels in the Community Library is not implemented yet, and the frontend still needs additional
work before it will fully support the Community Library.

The Kolibri side was not implemented during the project work.

## Follow-Up Work

Before moving the Community Library functionality to production, it will be necessary to extend the frontend user interface
of Kolibri Studio to support all features related to the Community Library. Then, the Kolibri application
will need to be extended with workflows for browsing and importing channels from the Community Library.

## Pull Requests

The following Pull Requests were submitted to the [learningequality/studio](https://github.com/learningequality/studio) repository as part of the GSoC project.

- 🔀 [CommunityLibrarySubmission model #5156](https://github.com/learningequality/studio/pull/5156)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet
    
- 🔀 [CommunityLibrarySubmission viewset #5167](https://github.com/learningequality/studio/pull/5167)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet
    
- 🔀 [Populate Country table #5168](https://github.com/learningequality/studio/pull/5168)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet
    
- 🔀 [Save channel included categories and expose channel version history #5176](https://github.com/learningequality/studio/pull/5176)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet
    
- 🔀 [Add action to resolve Community Library Submissions #5178](https://github.com/learningequality/studio/pull/5178)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet

- 🔀 [Add to community library on submission approve #5228](https://github.com/learningequality/studio/pull/5228)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet

- 🔀 [Ensure channel version database exists when adding to community library #5233](https://github.com/learningequality/studio/pull/5233)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet

- 🔀 [Add bitmask fields for ChannelMetadata categories #5272](https://github.com/learningequality/studio/pull/5272)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet

- 🔀 [Community library submission fields and filters in AdminChannelViewSet #5292](https://github.com/learningequality/studio/pull/5292)
  - ✅ Merged into `unstable`
  - ⚠️ Not in production yet

- 🔀 [ESoCC: Update UIUX of admin ChannelTable to support new Community Library info #5370](https://github.com/learningequality/studio/pull/5370)
  - ⚠️ Not merged into `unstable` yet
  - ⚠️ Not in production yet

- 🔀 [Submit to Community Library panel #5405](https://github.com/learningequality/studio/pull/5405)
  - ⚠️ Not merged into `unstable` yet
  - ⚠️ Not in production yet
