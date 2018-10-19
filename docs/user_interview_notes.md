# User Interview Notes

## Alex L.

Important considerations:

* When the API is actually being built (rather than discussed)

* When the API hits production

* When the API has actual users

* Blockers (such as ESCCB and ATO Process)

## Leanna S.

* Wanted to see this platform integrated with VA dev site

* Worked with a number of different APIs (including Appeals, Facility locator, and Veteran verification)

* Communicated to API developers regarding versioning and communication best practices (such as documenting release notes, etc.)

* Viewed a few different audiences/use cases for scorecard (such as showing current and future work, or showing internal progress to colleagues) 

* API phases were discovery, user research, prototype and design MVP, iteration, live launch

## Rachel R.

* Audiences were: Executive OIT leadership (Drew and Alex), VA executive leadership, and sample users (Rachel and Leana)

* Important considerations: API downtime and downtime of data source

* Interested in tracking lead times

* In the event of an issue, we would alert the business owner as well as Drew and Alex

## Alex L.

**1. What types of information about the existing APIs are important to you?**

* Existing APIs: current users, uptime, defined success metrics (such as transactions and error rate)

* Scorecard: technology and features that are currently in production and plans for future updates

* If APIs are a current work in progress, how close to complete are they in terms of their concept, a prototype, and proximity to launch

* I want to know if there are blockers that I could help them with. I’d also like to know what (if any) problems they anticipate to be upcoming, or else what they are currently  having issues with. 

**2. How do you go about currently learning about the states?**

Directly email those involved with the project and ask them questions

**3. What stages are important to you?**

The transition from concept to production and the point at which it has real users

**4. How might you define being built? Being scoped out, code, etc.?**

Not when you’re trying to figure out what backend system to use, or how to implement the platform; rather, it’s one of two other conditions. 1) when you know what your building (via a mock interface and iterating), OR when you write code for integrated development

**5. Tell me about decisions that informed API statuses?**

Knowing and recognizing when a team is blocked so that the problem can be taken to leadership (such as with a network connection, or a stallout as a planned launch day nears)

**6. Examples of blockers?**

* ESCCB - network connection

* Dependent on another team

* ATO processes

* VIP Processes - to release code, Veteran focused integration process

* Not knowing where to start

**7. Percentage of human vs technical?**

Not many technical, mostly human.

**8. Can you share what type of information you communicate up the ladder?**

* What features are being used

* What kinds of value the platform delivers to users and developers

* Demographics about the platform’s use (ie. if the platform is growing)

* Features currently being developed that may soon be released

* Business wants and needs in terms of how to continue development 

**9. Detailed run through of an issue for an API. How did you learn of it? How did you address the issue?**

* We were trying to launch the dev portal. In order to do that, we needed an ESCCB request to get the URL.

* I found out about that because I was speaking at a conference. 

* I called the people in charge of the process, explained the situation, and discussed the importance of getting everything resolved.

* Now, my current means of learning about issues is through daily standup calls because I am integrated with the project itself

**10. What are your thoughts on some of the tentative phases?**

* Would love to see a time metric (ie. ESCCB request made, granted, and how long it took)

* Options to add standards into the platform if something is red, as well as notes for what’s happening

* Would like log sheet of dates and times of different phases

* Like the prototype phase and like where that’s going.

**11. What would you want to know about when something goes cold?**

* It’s not a problem we face. 

* If the issue is a core reason the dashboard is being used.

* If teams are trying to use an API and they can’t. 

* Whether the system is deprecated.

* Whether we still have a team operating on a function.

* Whether the product owner is accountable.

* One or more available contacts for the issue.

## Leanna S.

* Product manager, VA API management platform

* Works on strategy and road map and oversees platform. 

* Handles primarily Internal APIs, but looking to provide external APIs, health data, etc

* A lot of these APIs were manual processes before. 

* Maintains a network of veteran service organizations that help veterans

* They have a developer portal with documentation for integrating with the API. 

**1. What kind of people are you managing?**

* Appeals APIs:  for call centers and other VA internal customers.

* Facility locator API: Facility wait times, satisfaction scores, info for google maps, mapbox, etc.

* Veteran Verification: Adjudicate/automate veteran statuses for jobs.

**2. When there are changes that happen to your API, how do you communicate?**

We’re new to the whole industry, only having operated since mid-June. We’re trying to follow versioning and best practices for communication. We publish multiple different versions of the API, document release notes of changes, and provide lots of notices

**3. What avenues are you communicating?**

Dev portal and github.

**4. How would you envision an ideal flow for communications?**

I think the scorecard has a few different audiences. One is showing what we’re working on and what's next. Another is to show progress for internal developers. Either way, the scorecard would be housed on the developer portal. 

**5. What kind of status info would you want to convey to your internal stakeholders?**

* It's not just about what APIs are live, we care about measuring the effectiveness of APIs and their impact.

* There is no list of APIs the VA has to publish. They want to uncover the most impactful ones. 

**6. Would the status be helpful to you? Metrics?**

These metrics would be helpful to executives in terms of answering two demographics-based questions:

* How many people sign up for a dev token but never put anything up to production?

* How many veterans are served by a particular API?

**7. Do you think there are universal performance metrics?**

Impact is hard to measure, but the percentage of applications that make it into production development is a good one.

**8. Describe the stages an API goes through.**

From our perspective, the stages are:

* Discovery

* User research

* Prototype and design MVP

* Iteration

* Go live

From a dev perspective, the stages are more like: when is the platform coming out. 

Some extra notes:

* We don’t need each task level of detail.

* We need to speak to Drew.

## Rachel R.

* Primary focus is on API strategy

* Currently moving into the health space with health APIs

* Member of a small team and working on multiple things

Important overview notes:

* APIs are ambiguous: it's a buzzword thrown around that creates a lack of understanding

* We can help track our own progress and help those who are not as technical in order to show them where they are and where they are going; this makes the concept of an API tangible

**1. What are the roles of the people you are communicating to?**

* Executives in OIT are technical, but don’t know what the APIs are for. 

* VA Benefits API, Cemetery Burial API, VA Health API: Business partners with whom we regularly communicate. They drive policy and requirements of the API, but may not understand things about APIs proper.

**2. What information do you think is most important for VA leadership to know?**

* The existing scorecards are pretty good (vet.gov scorecard, cloud.gov scorecard)

* KPIs: they’re a developer request (need to know how fast they are contacted)

* Downtimes of both the API and the source

* How many users are using the API

* If individual API scorecards were employed, there would be different metrics

**3. Can you talk about a time when you had an issue or blocker and needed to raise it to management?**

The biggest blocker is data integrity; if the data source goes down, this is a challenge because the customer doesn’t know where the issue is coming from. 

**4. Who is consuming your API?**

* For benefits intake, one organization that helps with claim processing (external to VA). Currently working to build and test.

* The developer portal is where they can get API keys.

* On the health side, we have developers, but no big consumer of the health data at the moment.

**5. What are your thoughts on issues with the lifecycle of the API?**

There is a general need for more communication and transparency. We should have readily available answers to questions like:

* When are we going to ship?

* Are things delayed?

* Is it done?

* What's in trouble?

* How do I know this is a good thing?

**6. Who is the most important audience?**

The three stakeholders:

* Executive OIT leadership (including Drew and Alex)

* VA executive leadership

* Our users: Rachel and Leana

	

**7. What frequency do they move states?**

We moved through the stages very quickly (we were built and running in 3 weeks), but some stay in the concept phase longer. Capital one tracks the lead time to see when things fall behind.

**8. Admin panels? What would you need to communicate up?**

Information like:

* How many users?

* Are there errors?

* What’s the downtime situation?

They don’t have a testing phase, so user research could be requirements gathering. We caveat things:

* Red is an issue

* Green we’re live

* Yellow prototyping

**9. If there was an issue today? Who would you inform and how would you do that?**

We would tell the business owner. We would need to tell Drew and Alex, and they would raise the issue up the chain of command. For internal APIs, we would just tell Drew and Alex. 

