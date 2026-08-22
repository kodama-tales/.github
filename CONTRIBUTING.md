# Contributing to Kodama Projects

This document defines the standard development workflow for Kodama repositories.

## 1. Track work with Issues

Development work should normally begin with a GitHub Issue.

Use the appropriate Issue type:

* **Feature** — new functionality or meaningful improvement
* **Bug** — something that is not working as expected
* **Task** — defined work that is not a feature or bug

Issues should include the relevant:

* Status
* Priority
* Initiative
* Assignees
* Start date
* Target date

## 2. Use Kodama Forge

Development work across Kodama repositories is tracked through the **Kodama Forge** GitHub Project.

Keep Issue status and ownership up to date so the Project accurately reflects current work.

## 3. Create a branch

Do not develop directly on `main`.

Create a dedicated branch for each meaningful change.

Recommended naming:

```text
feature/short-description
bugfix/short-description
task/short-description
```

When useful, include the Issue number:

```text
feature/42-customer-accounts
bugfix/57-email-routing
```

## 4. Keep changes focused

A branch and Pull Request should address one clearly defined piece of work.

Avoid combining unrelated changes into the same Pull Request.

## 5. Test your changes

Before requesting review:

* Test the functionality you changed.
* Check for obvious regressions.
* Run available automated tests and checks.
* Update documentation when required.

## 6. Open a Pull Request

All normal changes to `main` must go through a Pull Request.

The Pull Request should:

* Clearly summarize the change.
* Link the related Issue.
* Explain how the change was tested.
* Be complete enough for another person to review.

Use:

```text
Closes #123
```

when the Pull Request should automatically close the related Issue after merging.

## 7. Review

At least one approval is required before merging into `main`.

Reviewers should check:

* Correctness
* Scope
* Maintainability
* Security
* Testing
* Documentation
* Potential impact on other systems

Any unresolved review conversations should be addressed before merging.

## 8. Merge

Use **Squash and merge**.

This keeps the `main` branch history concise and makes each completed Pull Request one meaningful commit.

Delete the feature branch after merging.

## 9. Secrets and confidential data

Never commit:

* API keys
* Passwords
* Access tokens
* Private keys
* Production credentials
* `.env` files containing real secrets
* Confidential customer data
* Production database exports
* Confidential contracts or financial documents

Use approved secret-management methods and safe example configuration files instead.

## 10. Documentation

Update relevant documentation when a change affects:

* Setup
* Architecture
* Configuration
* Deployment
* User workflows
* APIs or integrations

The README should reflect the current state of the repository.

## 11. Repository ownership

Kodama repositories are company assets.

Do not create unofficial copies of company repositories under personal accounts for continued development.

Company work should remain within the `kodama-tales` GitHub Organization unless explicitly approved otherwise.
