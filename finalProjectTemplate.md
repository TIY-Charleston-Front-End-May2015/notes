### Name of project

Resource Linker

### Elevator

Allow anyone to post links and others vote on them via reddit styles, will have tags and other attributes so that the best links per subject bubble to the top.

### Technologies

- nodejs
- angular
- angular ui
- typeahead angular plugin

### features (MVP)

-  (1) ability to crud hyerlinks that other people can see and navigate to
- (2) ability to upvote on said links
- (4) ability to order links based on some sort of timeline type curriculum (eg. intro to js datatypes, then ajax)
- (3) resource types will have different attributes (eg. video, podast, image/infographic, tutorial, reference)


### Roadmap (for future development)
- mobile app via ionic
- user auth
- curation of own posted links and maybe add others links to their 'collections'
- mobile friendly app via responsive
- users can make comments on posted links, but will not be able to vote on comments
- web app also has companion google chrom extension so that one can easily add link to app without logging in via app.

### User Stories

 ability to crud hyerlinks that other people can see and navigate to

 ***
 name: create story
 size: med
 value statement: As a user of resource linker, I need the ability to post links as resource so that others can view something I found.
 assumption:
 - read, update, delete are covered in other Stories
 - assume navigation is handled in another story
 - assum that username is stored in local storage
 - assume that endpoint exists for posting data from web.

 acceptance criteria:
 - user can post to form that has following attributes:
   - name of resource (text)
   - url (text)
   - type (dropdown)
   - username (unseen by user, but code needs to retrieve by localstorage)
 - post form needs to have following styles according to wireframe (see notes)

 NOTES:
 Endpoint: POST - /api/resource/new
 wireframe: [Post Wireframe](../wireframes/resourcePostMockup.png)

 ***

 ***
 name: read story
 value statement: As a user of resource linker, I need the ability to post links as resource so that others can view something I found.
 assumption:
 - post, update, delete are covered in other Stories
 - assume navigation is handled in another story
 - assume voting is handled in another story.
 - assume that endpoint exists for getting data from server.

 acceptance criteria:
 - user can read resource, and follwoing attributes need to be present in view
   - name of resource (text)
   - url (text)
   - type (dropdown)
   - username (unseen by user, but code needs to retrieve by localstorage)
 - post form needs to have following styles according to wireframe (see notes)

 NOTES:
 Endpoint: GET - /api/resources
 wireframe: [GET Wireframe - listing resources](../wireframes/resourcePostMockup.png)

 ***
 update story
 delete story


######
 <User Story Template>

 Name: name of feature/piece of app
 Value Statement: As a <user>, I need <something> so that <VALUE>.
 Assumptions: what can we assume about this scenario.
 Acceptance: spec to which my story needs to comply with.

 Notes/Links to wireframes - please review #2332322 for more context

 #####
