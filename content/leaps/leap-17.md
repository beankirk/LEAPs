---
leap: 17
title: Establishing GrantsDAO
status: Implemented
author: Cinque (@Cinqu3), Burtrock, Ksett
created: 2022-02-03
---

<!--You can leave these HTML comments in your merged LEAP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new LEAPs. Note that a LEAP number will be assigned by an editor. When opening a pull request to submit your LEAP, please use an abbreviated title in the filename, `leap-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intend to achieve. This should be non-technical and accessible to a casual community member.-->
This LEAP proposes to establish a GrantsDAO.

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the LEAP is implemented, not *why* it should be done or *how* it will be done. If the LEAP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
GrantsDAO is a five-seat Committee responsible for evaluating and considering grant proposals for contributing to Lyra Protocol or LyraDAO.

##  Motivation
<!--This is the problem statement. This is the *why* of the LEAP. It should clearly explain *why* the current state of the protocol is inadequate. It is critical that you explain *why* the change is needed, if the LEAP proposes changing how something is calculated, you must address *why* the current calculation is inaccurate or wrong. This is not the place to describe how the LEAP will address the issue!-->
Community grants are a great way to reward contributors for providing meaningful contributions to the Lyra Protocol or LyraDAO. The GrantsDAO offers a sustainable way to reward contributors and transparency to these decisions. As Lyra evolves, sub-DAO's will help Lyra streamline the management process and promote stability and accountability for DAO's actions.

## Specification

<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->

### Overview
<!--This is a high level overview of *how* the LEAP will solve the problem. The overview should clearly describe how the new feature will be implemented.-->
GrantsDAO token holder vote would select Five DAO members, LyraDAO will distribute an NFT to the selected members to facilitate voting on grants and allocation of grant funds. GrantsDAO members are responsible for rewarding grants and allocating the GrantDAO funds.

### Rationale
Setting up a GrantsDAO is another step towards decentralized governance. This will enable LyraDAO to manage funds towards the betterment of the protocol and attract the talent, skills and, culture to develop and sustain the growth of Lyra.

### Technical Specification

Build a smart contract + frontend that allows GrantsDAO members to vote on grant proposals for contributing to the Lyra Protocol or DAO.

1. Grants

   	A grant is a financial award given to a contributor who provides significant value to the Lyra DAO or protocol
	- Anyone can propose a grant.
	- Accepting or Rejecting a grant requires a majority of GrantDAO member votes in favor (i.e., 3/5).

	The scope of the GrantsDAO in regards to grants include:
	- Defining processes and templates for submitting a grant proposal
	- Guiding applicants through the processes
	- Interviewing applicants and evaluating proposals
	- Voting on proposals and distributing the funds outlined in the proposal

2. Token Holder

	 - Token holders are eligible to vote in Grants DAO elections.
	 - Tokens that the Lyra DAO controls are NOT eligible to vote.

3. GrantsDAO

	The Grants DAO will be a five-seat committee and will sit for three calendar months at a time. The responsibilities of Grants DAO include, but are not limited to:
	- Being an active member in Discord and the broader Defi community
	- Recognize contributions made by the community members and reward them accordingly.
	- Attract talent and incentivize protocols and contributors to integrate with Lyra
	- Vote to Pass or Deny grant proposals promptly

	GrantsDAO position is an incentivized role and will be paid a monthly discretionary stipend by the LyraDAO.

4. Election

	The initial Grants DAO members will serve till the end of next council term.
	The GrantsDAO election process starts exactly after the council election ends. The election process will hold the similar election rules as the LyraDAO Council election. see [LEAP-15](https://leaps.lyra.finance/leaps/leap-15/).
	At the end of the voting period, the Five DAO members with most votes will receive an NFT from LyraDAO, granting them the right to vote on grants and allocation of grant funds.

5. Management of Funds
	
	Initially, grants approved by the GrantsDAO will be agreed on and funded by Lyra's DAO multisig.
	Once the Lyra treasury is established, $50,000 denominated in LYRA with a maximum of 250,000 LYRA is allocated to GrantsDAO each epoch. At the end of the epoch, any allocated funds that are not used are returned to the treasury.
	The monetary responsibilities of GrantsDAO include, but are not limited to:
	- Maintaining a budget in the GrantsDAO multisig contract.
	- Allocating funds to the grants that have been approved.

### Configurable Values
<!--Please list all values configurable under this implementation.-->
	Number of seats = 5
	DAO allocated funds = $50,000 USD (max: 250,000 LYRA)

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
