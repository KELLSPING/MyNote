# GitHub Precise Search

## Resource
* [Search on GitHub documentation](https://docs.github.com/en/search-github)

## Searching for repositories

* Search by repository name, description, or contents of the README file
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `in:name` | **jquery in:name** matches repositories with "jquery" in the repository name. |
  | `in:description` | **jquery in:name,description** matches repositories with "jquery" in the repository name or description. |
  | `in:topics` | **jquery in:topics** matches repositories labeled with "jquery" as a topic. |
  | `in:readme` | **jquery in:readme** matches repositories mentioning "jquery" in the repository's README file. |
  | `repo:owner/name` | **repo:octocat/hello-world** matches a specific repository name. |

* Search by repository size
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `size:n` | **size:1000** matches repositories that are 1 MB exactly. |
  | `size:>n` | **size:>=30000** matches repositories that are at least 30 MB. |
  | `size:<n` | **size:<50** matches repositories that are smaller than 50 KB. |
  | `size:n..n` | **size:50..120** matches repositories that are between 50 KB and 120 KB. |

* Search by number of followers
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `followers:>=n` | **node followers:>=10000** matches repositories with 10,000 or more followers mentioning the word "node". |
  | `followers:n..n` | **styleguide linter followers:1..10** matches repositories with between 1 and 10 followers, mentioning the word "styleguide linter." |

* Search by number of stars
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `stars:n` | **stars:500** matches repositories with exactly 500 stars. |
  | `stars:n..n` `size:<n` | **stars:10..20 size:<1000** matches repositories 10 to 20 stars, that are smaller than 1000 KB. |
  | `stars:>=n` `fork:true` `language:LANGUAGE` | **stars:>=500 fork:true language:php** matches repositories with the at least 500 stars, including forked ones, that are written in PHP. |

* Search by when a repository was created or last updated
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `created:<YYYY-MM-DD` | **webos created:<2011-01-01** matches repositories with the word "webos" that were created before 2011. |
  | `pushed:>YYYY-MM-DD` | **css pushed:>2013-02-01** matches repositories with the word "css" that were pushed to after January 2013. |
  | `pushed:>=YYYY-MM-DD` `fork:only` | **case pushed:>=2013-03-06 fork:only** matches repositories with the word "case" that were pushed to on or after March 6th, 2013, and that are forks. |

* Search by language
  | Qualifier | Example|
  | :---- | :----------------------------------------------------------- |
  | `language:LANGUAGE` | **rails language:javascript** matches repositories with the word "rails" that are written in JavaScript. |
