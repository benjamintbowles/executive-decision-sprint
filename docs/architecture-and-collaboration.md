# Architecture and collaboration

## Current application

| Component | Responsibility |
| --- | --- |
| React and Vite/Vinext | Landing page, guided intake, owner review, and customer Decision Room |
| Cloudflare Worker | Application endpoints and workflow operations |
| D1 | Persisted application records |
| OpenAI integration | Optional AI-assisted draft generation |
| Resend integration | Transactional owner and customer notifications |
| Sites | Current private deployment and managed access |

Human approval sits between the draft and its release. The exact customer preview supports the review. Customer-facing feedback and outcome capture are part of the workflow.

## Repository boundaries

This repository is public and contains a portfolio walkthrough, screenshots of fictional material, and documentation. The live application source remains in its private Sites-managed project.

The earlier public beta is a separate deployment. Updating this portfolio does not deploy application code or replace that site.

## AI4VA practice kit

The portable teaching copy provides fictional cases, installation instructions, focused local tests, and instructor guidance. Students should receive that scoped copy through a separate private collaboration repository or an instructor-provided package.

The intended student work includes:

- Map the intake and review workflow.
- Compare approaches to simplifying intake using the same sample cases.
- Check whether material evidence, assumptions, and decision constraints survive simplification.
- Report usability problems and propose prioritized improvements.
- Make changes on branches and submit reviewable pull requests.

The practice kit is portable across development computers and can support a separate Cloudflare deployment. It is not a static-only website or a drop-in server for every hosting provider. Dependencies need internet access for the initial installation.

Production credentials, live customer records, deployment destinations, and unrestricted email access do not belong in the student copy. Optional external services require separate instructor configuration.

A dedicated GitHub source/collaboration repository is separate from this public portfolio. This page does not imply that a student repository has already been created or that students have been granted access.
