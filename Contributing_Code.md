Contributing Code
===========================================

Open source software is driven by community contribution, and one of the most effective ways to participate is by contributing code to either the [MongoDB Server Repo](https://github.com/mongodb/mongo) or one of the [many related projects](http://docs.mongodb.org/ecosystem/drivers/) such as drivers and libraries.

###Guidelines for Contributing:

####Pre-Pull Request: Searching for Issues

Before you submit a pull request to the MongoDB Server or any MongoDB open source tool, please review the [open tickets in Jira](https://jira.mongodb.org/browse/). For Server Contributions we suggest reviewing the [Server Roadmap](https://jira.mongodb.org/browse/SERVER#selectedTab=com.atlassian.jira.plugin.system.project%3Aroadmap-panel) on Jira to find issues that are scheduled but not assigned. These will improve the chances of your patch going into a future release. 

For upcoming releases, issues are ordered by "fixVersion":

- “2.#.#” are things we want and have scheduled.
- "2.#.w" are things we want but don't think we have time for.
- "2.#.x" are things the Kernel team wants but *really* does not have time for.

Avoid tickets with fixVersion "Needs Triage". This is the default fixVersion for new tickets, and it indicates that no decision has been made on the ticket request for the roadmap.

#####Pull Requests to the MongoDB Server

Before you submit a pull request to the MongoDB Server, please complete the following:

 * Read the [guidelines for contributing](http://www.mongodb.org/about/contributors/).  In particular, you should ensure your changes adhere to the MongoDB Kernel Development Rules such including code style, exception handling, logging, and tests.
 * Identify an existing [SERVER ticket](https://jira.mongodb.org/browse/SERVER), or create a new ticket for your pull request in the Server project. Please include a reference to the Server ticket in the title of the pull request (eg: "SERVER-1234: Add $foo operator to Aggregation framework").
 * Make sure your code request is specific to the changes in a single Jira issue.  If you have made multiple commits, it would be preferable to [squash](http://git-scm.com/book/en/Git-Tools-Rewriting-History#Squashing-Commits) these into a single commit before review of the pull request.  If your change fixes multiple Jira issues, either split these into discrete pull requests or include some detail on why that is not possible.
 * Sign the [MongoDB Contributor Agreement](http://www.mongodb.com/legal/contributor-agreement).

#####The Life-cycle of a Pull Request 

When you submit a pull request, here is what happens:

 * The engineering team will review your pull request to make sure you have included a SERVER ticket in your request and signed the contributor agreement.
  * You should receive a response from one of our engineers with additional questions about your contributions.
 * If your pull request matches a ticket and is aligned with the Server Roadmap, it will get triaged and reviewed by the Kernel team.
 * Pull requests that have been reviewed and approved will be signed off and merged into a development branch and the associated Jira SERVER issue will be resolved with an expected fixVersion.

####Best Practices

* Never introduce breaking backward changes.
* Write inline documentation (comments) so project maintainers and others can understand your code.
* Write tests and make sure they pass.
* Make sure your code does not break any of the existing tests.
* Review the appropriate project license. To contribute to the MongoDB Server, you must sign the [contributor agreement](http://www.mongodb.com/legal/contributor-agreement).
* Add yourself to the contributors list. Most projects have a [list of contributors](https://github.com/mongodb/mongo-hadoop#contributors)
on their Github READMe. Once your patch as been accepted, add yourself to the list. 
* Read the contributing guidelines for each project. These can be found in each individual driver repo and may differ across project. Also see the [full list of drivers projects](http://docs.mongodb.org/ecosystem/drivers/).
* Show off your accomplishment by [requesting a contributor T-shirt](http://www.mongodb.com/swag) once your first patch has landed.

If you need help or advice, the [MongoDB-user](https://groups.google.com/forum/#!forum/mongodb-user) and [MongoDB-dev](https://groups.google.com/forum/#!forum/mongodb-dev) mailing lists are extremely active, and both are good places to either ask questions or learn from others' experiences. MongoDB-user is for users building applications with MongoDB, whereas MongoDB-dev is best used by those contributing to the database or building third party tools. Also be sure to check out the #mongodb IRC channel on Freenode, or tag your question with mongodb on [Stack Overflow](http://stackoverflow.com/questions/tagged/mongodb). If you can answer another users' question on any of those sites - feel free to jump in! 

Always remember: MongoDB is developed in the open. The source code can often be the best way to understand how it works.
