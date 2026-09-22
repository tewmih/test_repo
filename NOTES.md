# Co-author attribution test

Question: does a `Co-Authored-By:` trailer make the co-author appear in the
repository's contributor list (Insights → Contributors)?

Method: this branch carries one commit authored by the repo owner with a
`Co-Authored-By:` trailer naming Claude. Merge the PR, then check:

1. The commit page — is the co-author shown, and is the name a link to a
   GitHub profile or plain text?
2. Insights → Contributors — does a second entry appear?

Note: GitHub resolves a co-author to an account by matching the trailer's
email address to a verified email on some account. `noreply@anthropic.com`
is not registered to any account, so it can only ever render as plain text.
