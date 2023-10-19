# GIP1: Managing GEODNET Improvement Proposals

- Start Date: 2023/10/01
- Original GIP PR: 
- Tracking Issue: 
- Authors: GEODAO Foundation

# Summary

Defines an initial process for proposing, discussing, and finalizing improvements to the GEODNET
network using GEODNET Improvement Proposals (GIPs).

_"How a bill becomes a law"_

# Motivation

As GEODNET Foundation begins to share control over the development and management of the GEODNET Network,
it's become clear we need a community-driven process for making changes to the protocol, network
configuration, and other shared concerns. Fortunately, we are not the first to this problem, and
this document draws heavily on the the Improvement Proposal processes of
[Ethereum](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1.md),
[Zcash](https://github.com/zcash/zips/blob/master/zip-0000.rst),
[Rust](https://github.com/rust-lang/rfcs) and others.

This document aims to outline a process that is transparent and inclusive while remaining as
efficient and pragmatic as possible.

We do not aim to adjudicate routine technical changes to miner software or the day-to-day dealings
of GEODNET Foundation. We expect that any change that could have significant impact on the functioning of
the GEODNET Network would be vetted through the GIP process.

# Stakeholders

We plan to circulate this proposal in
[Discord #GIP-open-discussion channel](https://discord.gg/geodnet). We will also solicit specific
individuals for feedback, from both within the GEODNET community and other crypto and open-source
projects.

Specifically we aim to achieve rough consensus around this process with GEODNET Foundation (as the primary
developer of nearly all core GEODNET software) which plans to commit time & money to community governance in the
GEODNET ecosystem.

On-the-record comments should be made on this GIP's [associated GitHub issue](TODO). As described in
this document, that issue would be opened automatically after this GIP's initial pull request has
been merged by a GIP Editor. That role is also described below.

# Detailed Explanation

## Overview

The GIP process generally starts with an idea for improving the GEODNET protocol or modifications to
network configuration. GIPs can also cover improvements to the GEODNET. 

The GIP's author is responsible for building support and consensus for their proposal.

There are three major types of proposals:

- _Technical_ – network and protocol upgrades
- _Economic_ – modifications to rewards or incentive structures (generally via chainvars)
- _Meta/Process_ – changes to the GIP process itself; presumably would also include processes like
  the selection of committee members and the induction of core developers

We propose the creation of several roles to help facilitate this process: _GIP Editors_, who
administer the GIP process, and _Review Committees_, who serve as specialists for technical vs.
economic proposals and operate as a first line of feedback.

## Submitting a GIP

In the earliest phases it's best to vet an idea with the GEODNET community
[via Discord](https://discord.gg/geodnet). This is a good way to see if there is initial support for
the idea, or if it's been discussed before.

After vetting the idea, please write it up using this markdown-formatted
[GIP template](https://github.com/geodao/GIP/blob/master/0000-template.md) and submit it as a pull
request to this repository (`GEODNET/GIP`). The current template is geared towards technical
proposals, but can be adapted for economic or meta proposals.

How to submit a pull request:

- Fork this repository (e.g. using the GitHub "Fork" button top-right) and checkout your fork
- Add your file and give it a title but do not allocate a number, e.g. `GIP-data-credits.md`
- Commit your changes (`git commit [filename] -m "Description of your changes"`) and push them to
  your fork (`git push origin master`)
- Submit your change as a [pull request](https://github.com/geodao/GIP/pulls)

Within a reasonable timeframe after you've submitted your PR, a GIP Editor will review your pull
request.

The PR will be merged it if it adheres to the standards outlined in this document, which formally
opens it up for consideration.

If there are issues, the GIP editor will provide feedback. The feedback at this stage is intended to
be logistical, rather than on the actual contents of the proposal.

## Discussion and approval process

_TODO this could use more detail; feedback & contributions very welcome_

- When ready, GIP is scheduled for discussion on a community call.
- Comments should be put on the GIP's associated GitHub issue, and/or
  [GEODNET Discord Community](https://discord.gg/geodnet)
- Approval is achieved through
  [rough consensus and running code.](https://en.wikipedia.org/wiki/Rough_consensus)
- GIPs have a status: _Draft, In Discussion, Approved, Deployed, Rejected_
- If a GIP goes stale and discussion is dormant, it should be closed.
- When rough consensus is achieved, a GIP is marked `approved`
- When a GIP has been merged and deployed, it is marked `deployed`.
- GIP Editors are responsible for keeping `geodao/GIP` repository groomed and well-organized.

## GIP Editors

As mentioned above, we'll need people to help organize and facilitate the GIP process. This is an
administrative role, and Editors are not arbiters of what does or does not get approved.

Editors would be responsible for:

- Reviewing new GIPs submitted to the GitHub repository
- Flagging issues related to formatting and structure, but not commentary on its substance; that
  should be reserved until after the GIP's pull request has actually been merged.
- Evaluating community consensus and updating GIP statuses accordingly

## Review Committees

We expect different stakeholders to be more interested in Technical vs. Economic proposals, and so
we suggest the formation of Review Committees for each of those tracks.

Review Committees would be expected to meet regularly and discuss GIPs falling into their area, and
in conjunction with GIP Editors, help keep the improvement process moving.

The committee is an informal group and anyone can join one of the calls and make their voice heard.

Since there relatively few GIPs and no clear members for any given committes, the newly launched
GEODNET community calls can serve as a catch-all for reviewing proposals.

# Unresolved questions

- How are Review Committee members selected? Open to anybody or elected or other?
- How are GIP Editors nominated and selected? (Related: Who currently has write access to
  `geodao/GIP`?)
- How do community calls work? It's assumed in this document these will occur regularly and be open
  to the public
- Who are the current core developers? Who has the ability to merge code into core repositories?
  What are those core repositories?
- Who has the ability to deploy changes to the blockchain, and the related responsibility for its
  uptime?
- How long should a GIP be allowed to remain in a given state?
- Should we encourage people just to leave comments on GitHub, rather than trying to track GitHub or
  Discord?
