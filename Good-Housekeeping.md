# Delivery Schemes

A particular delivery scheme performs the routing of messages between nodes in a network. How we communicate as individuals at work has clear parallels. Examples of delivery schemes are:

-   Unicast: This delivers a message to a single specific node. Think of this as sending a DM or an email or having a private conversation.

-   Broadcast: This delivers a message to all nodes in the network. This is similar to an all-hands meeting or an email to the staff-wide mailing list.

-   Multicast: This delivers a message to a group of nodes that have expressed interest in receiving the message. This is like a skill-set–specific public chat room such as #backend or #datascience.

-   Anycast: This delivers a message to any node out of a group, such as asking someone walking past if they can sense check how you’re trying to debug a problem.

# Conway’s law

states that “organizations that design systems are constrained to produce designs which are copies of the communication structures of these organizations.”

# What is a guild

A guild is a group of people who work on different teams but share a common interest or skill set. The neat thing about guilds is that they’re just a group of people with a common goal.
The reason they’re worth covering is that they’re another useful tool for you to suggest to your staff to solve common problems, which in turn increases their confidence and autonomy.

# Purpose of guilds

-   Discussion and progression of best practice across an interest or discipline.
-   Information sharing across multiple teams.
-   Improving the visibility of that interest or discipline within the company.

# Five Whys

A five-whys session is an excellent way of determining the root cause for an issue by repeatedly asking the question, “Why?” The number of whys is unimportant, but five is usually enough to get to the bottom of an issue.

For example, let’s assume that your application went down for a period of time and a patch was required to fix the bug that was causing it.

Before the team moves onto whatever is next in the work queue, get them together to interrogate the problem. Get around a whiteboard or a shared document and begin questioning:

-   Why did the application go down? Because the API stopped serving any requests
-   Why? Because the latest deployment caused a deadlock when the application started up
-   Why? Because the production environment has many more concurrent requests than the testing environment, and a non-thread safe data structure was used
-   Why? It wasn’t thought about during development. The tests all passed.
-   Why? The automated tests don’t cover any high-throughput scenarios.

As a manager, performing five whys has a number of benefits:

-   It determines the root cause of a problem so it can be fixed.

-   It educates the whole team on what these issues are so that they can be avoided in the future.

-   It reinforces that whatever happened that triggered the five whys is the kind of behavior that you want to avoid in the future.

-   It helps to identify patterns and trends in problems which may not have been immediately apparent.

# Tools to Solve Common Problems

To prevent problems where you can’t remember why your code wasn’t written differently., you can use an Architecture Decision Record (ADR).

an ADR should capture

-   The point in time in which the decision was made
-   The status of the ADR (proposed, accepted, rejected, and so on
-   The current context and business priorities that led to the decision
-   The decision itself (What are we doing as a result of this?)
-   The consequences of making the change, such as what is now easier or more difficult as a result

You can store your written ADRs in a place of the team’s choosing, such as in a folder on Google Drive, or, you could check them into a top-level folder in that particular codebase.
