# Rust seed application

It's written in Rust!

This is a framework for building Rust applications in combination with building Docker containers and never rebuilding code on release, instead we promote existing code.

## TODO and done

-   [x] Figure out how to deal with PRs pushing too many Docker containers

    > We only build containers on the tip of the PR, so even if you're pushing 10 commits, we'll only build one.

-   [ ] Remove old containers when the new one gets build for a PR? Or rely on a general weekly untagged cleanup?

-   [ ] Remove PR containers when PR closed

    > API currently unavailable

-   [x] How do we deal with older containers on `main`?

    > We move tags, so we'll need to wait for the API to clean up untagged versions
