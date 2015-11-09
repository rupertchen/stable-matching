# stable-matching

## What It Solves

- Proposes stable matches between Sets A and B
- Individuals in A and B provide ranked preferences for matching to the
  other set.
- Returns multiple proposals such that previous matches from 0 to N-1
  iterations are avoided.

## Additional Tools

- It is more and more expensive to require complete preference lists
  from every individual as the number of participants grows, so
  provide an supplemental syntax to express groups that can be used as
  shorthand for arbitrary blocks of preferences.

## Example: Selecting peer reviewers

One such use case is in the assignment of peer reviews within a team.
Both reviewers and reviewees provide their preferences for who to
receive reviews from and who to review, respectively.  Groups are
defined globally and can be used by participants to "block fill"
contiguous segments of their preferences.  The tool can then be run to
select N reviewers for each reviewee.

## TODO

- Set up dev environment for Go
- Implement Gale-Shapley algorithm for single match
- Implement iterations for additional matches
- Implement configurable bias-ing
