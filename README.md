# API Testing Portfolio

## Overview

This repository demonstrates API testing using Postman and REST APIs.

The goal of this project is not only to learn Postman syntax, but also to demonstrate QA thinking through:

- Business goals
- Risk identification
- Test design
- Automated API validation

The project follows a risk-based testing approach. For each endpoint, the business purpose is identified first, followed by potential risks and automated validations.

## Repository Structure

```
api-testing-portfolio

├── collections
├── environment
├── screenshots
└── README.md
```

## Tools

Postman
REST API
JSON
Git
GitHub

## API Under Test

JSONPlaceholder

https://jsonplaceholder.typicode.com

JSONPlaceholder is a public REST API used for learning and demonstrating API testing concepts.

## Testing Approach

For each endpoint:

1. Define the business goal
2. Identify risks
3. Design validations
4. Implement automated tests

The intention is to demonstrate practical QA thinking rather than only technical API requests.

# Implemented Test Scenarios

## GET Post

### Endpoint

GET /posts/1

### Business Goal

Retrieve a specific post by ID.

### Risks

- API unavailable
- Wrong post returned
- Missing title
- Missing content
- Invalid response structure

### Validations

- Status code is 200
- Returned post ID matches requested ID
- Title is not empty
- Body is not empty

## GET All Posts

### Endpoint

GET /posts

### Business Goal

Retrieve all available posts.

### Risks

- API unavailable
- Empty response returned
- Missing required fields
- Invalid response structure
- Validations
- Status code is 200
- Response contains one or more posts
- Every post has an ID
- Every post has an author (userId)
- Every post has a non-empty title
- Every post has content

# Planned Test Scenarios

## POST Create Post

### Business Goal

Create a new post.

### Risks

- Post not created
- Missing required fields
- Incorrect response returned
- Planned Validations
- Status code is successful
- Created post contains submitted data
- Response contains generated ID

## PUT Update Post

### Business Goal

Update an existing post.

### Risks

- Changes not saved
- Wrong post updated
- Invalid response returned
- Planned Validations
- Status code is successful
- Updated values are returned correctly
- Post ID remains unchanged

## DELETE Post

### Business Goal

Delete an existing post.

### Risks

-Post not deleted

- Incorrect response returned
- Wrong resource affected
- Planned Validations
- Status code is successful
- Delete operation completes successfully

# Portfolio Notes

This project focuses on demonstrating QA analysis, test design, and API validation principles.

Where appropriate, validations are based on business expectations and risk analysis rather than solely on static demo data.

The purpose of the project is to showcase practical testing skills that can be applied to real-world APIs.
